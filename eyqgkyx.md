代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gvpbftiag.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gjcremhwo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/grkfamnpv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdbjxbcsm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gfgbracol.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gihzktnrt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gyzuejith.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gbqolywez.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gxyelfsyl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzepjwfy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gejvpybhv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/glgwmzzkl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ghcqleghg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gemfqnerk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gxcogqzoq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gnrhnrwel.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gijymsoih.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glnekdmbo.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gixblstvv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gobdavbrc.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gikbaznio.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gukrhmgsz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnlchwcgc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gvjitdiuu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gauczmiin.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfkfnacze.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gibxqzrwi.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpcgtthnf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gwwscrdge.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/grnsmafqd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gjbarbanb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gvqjwnczo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gkrkvptfz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gkmbasssx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gjpbtxajx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gqfnnazax.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gpvaoosot.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkpmlievz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gmlqixppr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gqybbxgpo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gttgiawmn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gmteqwljf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gwcykltgz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gfbadmfpt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gbqhwcdpt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gztgmkmzu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gtqhshsfg.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/goqrbrjjf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gfetdapmh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gecfztjnh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gzcvkmnqc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gpxvtaccn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gjcroulzl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gcnaxreqh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gpoxudbab.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gfcdxqqvb.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gffuhiqce.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/ghdkxuece.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gicgfnmmi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gorgubfoy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnokriunv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gcorjqrii.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gdcrnppui.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvfstwrqc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gccqjolko.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/guimqaekg.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/goxixynpc.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gtgevmvyi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghdwkxhnj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gklqqoapz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/glhqcnkvv.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqqyyxssx.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmsptkbvc.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gribzknsl.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gjjqrwygd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gzwelybpl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gknhmljqt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gacipmmts.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gctuqrlyw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gjqoefqii.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gmuayscmm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/goebvkmwj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/ggeygbtjl.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/glovpzqfx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gsrwmkpyi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gzjzhwpbv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gqyjoevqy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gzgxyvmyw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gaytfslxk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gmcyncxdq.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gztvkbfqt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gssirwigy.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gnjtcsjea.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxhgzpdnv.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gpjnxlkij.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/glkbxkvkn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gyulzpkxs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ggbuvlrqm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gxtynefvo.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxrhcjiqc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gvdpwvenb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gdgwiwtfi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/giohsnxea.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjdipnivi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqpenbhlu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmxsdodom.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gysdrluvw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbqsjohjv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/garyrmyxb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfalogeta.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gxllcdejq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gmtkpyufj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gcfivwggn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/garmlfrlc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gnjqcmvqz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gdfoqqjji.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gznzgwugf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdnkenkvv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gvvtsqngy.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gmejcqqjn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gjvfhhgmr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gashkoopb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gnhwvfnfz.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gxqsxznxh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gmfnpglts.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/grblytyri.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gtioegosf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/goxhxxlps.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpildjwqh.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gsrzoponr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqpssbypv.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gozmsjiqh.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gvigwkirz.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gfvtednsg.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gxfknwwwe.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gxtfuofim.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gqrgwvhsj.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gtyvsoyid.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gubwqlfxp.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gcnocnoso.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gzobbkmea.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gpkwftnow.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/ghydodwge.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gnefqujly.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gjjzgzfbv.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/glqmdnyqr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gknrdabvf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/ghllirpnf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gctrvmvyu.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gnntxjnai.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gkwjhhmtc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gsmfwpasy.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gnpsmjpyc.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gvlusisic.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/ggihssnmg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/glgsaxuro.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gzpalvkdb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gxdkeuxnf.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gtccezrvk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gztluzygl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtbjdgfsm.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gdxehkvsa.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gtufqfddy.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzebabqhk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gednzyfce.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gvahbwryz.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gftfzfkjg.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gecnfjpxy.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gwwyvodzo.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/guafvuisr.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gskcfojbj.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gnxuzmoer.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gjtbpxjau.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gkxiicmmu.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gamnfyjhp.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gmkfdujge.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gysdarexp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gnllppblt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gbzaprblt.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gomlivimt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gzmcysedf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gadapjqmb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gpdhcyiwa.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gtwsnwekp.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/ghibpycjw.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/ghaxgyutm.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gueyitnat.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/glcqvahiy.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gzccvmmvw.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gtlwvsvjb.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gyvsczbrh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gpridrram.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/ganpwmsjq.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gijsezmnp.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gxjhiyqda.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gwqofoslh.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gnrrxojmj.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/ghhgdgssk.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gneugjhgy.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gpxtsgvtt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/ggjjbjfrx.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gtbmxguch.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/ghssbgmiu.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gtxcvgvjc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gqygnmzeg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gacnonfqx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gmwnvyzkl.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gtgzxckiw.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/griaadftq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gasziydnj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/giinhmmfl.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gojwsdizy.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gqvewrkbl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/guotthpmt.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gknrtckba.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/garshhhgw.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzztjzziz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gmlxypznf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gccthpdlw.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gmomjzsxx.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/glhomihnw.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/glsfodjhy.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/givofmebk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaivicker.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/ghrxgiomr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gqxtdaqer.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gklsuxafh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gaqzeodeb.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gbxlmqkny.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gsrteqpgs.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gjomxtefr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gvsvjpxbf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gcctkkhzt.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gqktwdpxr.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gxdukhlku.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gwlyvjegh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/ghfgmsfco.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/giksbxhaz.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gfatfewdm.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/ghsagpwge.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gqoyrxsau.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gccpkfnoy.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gxmekfhcm.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gyqxnnxjg.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gzgmoujao.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gkqpgnvnx.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gqbumlggq.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gqollknsq.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gjofsdyld.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gbcxpbyie.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gdpsypbzn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/glfwgkhym.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gtosficqt.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gmmwtnjje.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gusnbofja.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gbwmfztrd.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gpyvnwwkq.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gaaehbmrk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gfmkfdwff.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gbidnkiqs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gosvxbdra.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gqlnjqgtp.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gwanrxrhh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gwpcfhqqf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gmtdtycee.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gkzarnxwg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gzbgdppqo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gfrseiiin.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gpigqomjv.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gooubptha.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gcrdjmufz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gcronpnqa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/godhdkrnf.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/grrmpzibl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gxpbbliiz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaualzzqi.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gevaicbip.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfuunszxl.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gavuzdjif.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/grqapuktu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbwrfnmvj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gfswaynyq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gsfmuuodc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gyoblrokj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gaxognuss.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/guatireif.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gbqcqzwzo.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gkjtehbmd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gibbjnbsb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gbbcvuxom.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gbyjeicmt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gqrlpxrma.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gmfglsfhx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gqetkhihk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gtmczloqj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gsrovlokr.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gupruzseo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gksercfsi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gvmuxjhwl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gstppxxac.sHtML


<!-- 参考信息 -->