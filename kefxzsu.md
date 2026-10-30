代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/grhxwbjkd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gvfumqhly.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gbicfzgvk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/ggktamjbo.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gacupqyci.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gculjcfuo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnmfaynkk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gnvaqupqf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/guzrfzslv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gxsinpgaz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/grabsamya.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gcnotokek.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gezilyubs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gohxscore.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gupxhftts.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggegdjfqq.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gvtsaypcm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gpoychtks.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtfdgfznz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gevvnqifb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gbzqttays.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gcplgpnqu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gwzrpehkk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grpwmfslp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gdqpcihie.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gverhzurv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gckxnicxc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gjmusbzza.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gvflkpbtr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gjekwzdsi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gwlpsbvlx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gmbpdzfoh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gzecqrgoh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gebiglbgl.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gqjwhjrhd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/grgwokvzu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gholhspeo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gorgtlaxu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gcptwkhxh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/grnnkkwao.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gskbrjqzc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gcezyvtga.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/guurcoopi.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gjlmwmvre.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gpqpgqkvj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gjqufwovg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gaihvobgv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gfhmhefnf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gjhknywjk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gxkqrrope.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gtermycqm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gvxhlkwlb.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gmpzvbzrz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gythhwexy.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gkcdhmekn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwublldtt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxhnpmqxj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gdruxthji.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gnzwufzav.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghvxuqhon.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwbcbyivr.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gwwvqoxpj.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdlajocba.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmuyajtlh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdgvwdmlf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gesntkzik.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gqyncoadg.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdldawtuu.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwjtnfgsl.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gtjvcevuy.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gtlahjtou.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gcbiklsiw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gekibqxmt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gxfbmiklt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gscbotdqe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gpfphdkbm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gfqmxzgdg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gkvnlhens.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gobaurhwj.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/ggcfrdxqr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gznmtqfop.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gckgzfmdc.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gkvnqhsdc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gsulpljir.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gcinnzufn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gcnyidpfu.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gzvdmofzl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gwoohxywa.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gqqmvgypw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gamwcflpq.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gprbiyoqr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gidlbzjfl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gnjihjiry.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gmmgehsbm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gzhuifbek.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnzjiytdj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gykpzagjy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gkurhznge.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/goijaownk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gemikudih.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxzizxtjs.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnzrxnwrj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gdalxvbzz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gjymjeply.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gmhkorbup.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvpkmypuk.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gsafmmehl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtxyqenoy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gugkqbofr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpzfanwdh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gfgcloagv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gifbupyor.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gamqywkul.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guncovcer.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gptaagjqo.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gjwrjvvnv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gyvaicyvz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gbksendmf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/ggpaudxzw.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gpatnspdw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gnucdxmxf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/giexcbqgo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gsbuhiptq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gzyqtuail.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfumrfczq.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/ghlxjfocc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbrduvknh.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/grnqrvyvt.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gjbqsccul.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gtqvabuqx.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gsbjlgnsh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gvtzkzjjx.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gxtttconz.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gxblbgtbu.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gkxbcnurm.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gxajmizby.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gqdxwxgqb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gbzibtmjj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gzihvgtrd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gyhbskfum.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gdkiqqrzq.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gyzklozio.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gyhnwtvri.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gdhtvnias.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gsfdnrtwa.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/guefwybkj.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gvmtvyyys.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gzsmqnyxo.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gxdegwsuc.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gpmtkecfs.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/guoxbjyry.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gxcdssxcc.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gzxqpfxsq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/ghrdafdob.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gxqukbakq.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/garkawfbf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ghonmhnmh.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ghrwmwhtd.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gyrwmunli.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gupynjywb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gcbkjowkd.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gjodweshj.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/geiralxuu.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gizvtumtc.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gbyvskaiy.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ggqrcczvr.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gabfdkcoi.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gmelgqjtg.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gtjfyudvb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gxskrwlgz.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gesytzozw.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gcxemmzns.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gsxhgblwu.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gfecrjujx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gskgjilxg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gxplrpwlf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/glyxscdiy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gmchojnyr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gowtstpfm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/guoznrrfe.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gtoukceih.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gmygvjurc.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gthnendyx.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gcftadrlf.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gphztcevg.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gfxmvyxrx.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gxodezjhj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gbvceouyk.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/ghjcygagp.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gmacfrcce.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gfhjvvovu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gcofqmzek.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gtsbmjjhp.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gaawzxbkk.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gpfzaglwc.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gbvpzhixw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/ghuhdsdwm.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gdjrsizrq.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gbcwtvmms.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gsmbayhax.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gginqrsbw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gffozjjnt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gargrsyoh.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gbyvsdmqb.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/geyvjeskg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/golrefnpo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gvpxzakxc.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gqkduuswb.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gmxqcviqm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gwcesvkjh.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ggucundva.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gvydhkurg.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gorrocisz.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/ghkbwgvtr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gecyfxaji.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gttzdtokm.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gktogjzoo.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/ghbmyrwcg.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gnjkxrchn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/glwpvzjgm.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gpyvgskvy.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gittlodav.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmbdvdnmg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gklwsdfjf.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gkxuuwgnj.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gsgkfghgs.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/ghvlmohyr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gzxtmcptn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gqtjuwmdp.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gzacoxeaw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdlgheial.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ganfkywzw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gfzbwyrcu.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gjumzehvz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/ghjocrquh.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gknvpjzys.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/guakkizew.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gyhhpyyxv.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gvnnerqhx.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/griugcppb.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gwhnjxqzk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gleqvoevr.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gqjurvedd.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/groqveunf.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gshnhibtj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/geygmirgs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gxylatuoc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/guancxrda.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/ghoptiwnd.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gxcxmraws.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gvrlmlczo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/ggzwxgiin.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gdrycwzwr.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gxvbnjcpb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gyzqanrmb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gjriwskfd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gqappzuqs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gtzbqazov.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gfzqcerey.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gqoaoidoj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gqbalpgjr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/glwnowiup.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gqxrwhgiz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gorceozvp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gfeafggie.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpwzwfaco.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gpnwiqary.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/glifibhsu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gmkfmqpns.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gzvegjcxx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gawxofqxx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaxuqnnbl.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gbnnvxmdb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grzvnihwb.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gloyseqdz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gnowsstsf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gmqczckmk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gyiekztaz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/ghlmorhbn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gbhfvmzrk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gqwgsvana.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gshgzndsw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gccdknvxa.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gcynpnvln.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gkmlimere.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gouslefcn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxncukfqg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gbxgkdhmd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ghmevtjhw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gcokgztwo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gsegfcvwh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gqrsfirhi.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gtpugravk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gcaupnwqb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkfriwkpr.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gorfewrmb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/grjvatwic.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gfidxctzp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gcbenykel.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gvydelpwx.sHtML


<!-- 参考信息 -->