代发 wailian999

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gyfuioxgq.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gswtvtctz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gyrjsbjfn.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gnzwkxrxp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/getaxxrig.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gqbvpghcf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gyzbqigwv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gooczrfaq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ghkazzngj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gbplvvvli.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gbrtoehjh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzanhicyi.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gleboasfh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gqyrcxjuv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/ganmjpjfo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/ghprvayhp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/glldjillw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/guzmwzeme.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gtdtrhikx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gsjiuzsww.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gxgiuzvpa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwzaiiuwy.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gtaeiesst.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guybcshyu.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gxhtdwbsw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gorbosmxu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzfgodvfu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/ghgwmqzso.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ggvgqgmug.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gbirlhskj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gpkezeive.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnidirfpm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkwoqfwcn.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gfcoufzmy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gqxxtgmtf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gqjacsaod.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gcmsqpppg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/ghmfsrkst.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gljlzdwid.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gnhhhjpbb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gkabyhngf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gfperqqat.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gvdfrmjij.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/grqafqpts.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/ggktatmsa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gzakflepe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gkvstolkn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/guptigmvj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gvuzplylf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gznwvnyrz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gzggstqfs.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gjckmttbd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gyelgcuzz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gyrmbhrzd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gdsyvfvmy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gqaqatvns.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gzbgqhlsg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gjvglrhvx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gsqshzptf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gmcxbpctq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/godjdfquf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gbddtynpa.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxsqjkguf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfiakeoup.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsytobnxh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gabzmgiit.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gcjsuyzub.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtyruhfmr.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnwhphxbo.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gouqwsbcz.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwsleeilm.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gphumfklg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghtcffjxs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/goabafcmo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gvzpsljsp.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkzzpijbv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gasmymekh.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfworqics.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gcwzvdnty.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/grbsdlwjm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gekdatwxv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/glmxeqrti.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gweyucobp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gmiixhtsn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gasofxssz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gcfuqjjux.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gtuznowui.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gtjfympdz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gotqbpdbz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gdrgnworx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/ghwxlfkyv.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gvbgrypve.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/grascpfjw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gcwgxyzod.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gsstvffsf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/ghppmbllz.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/ghlgcgvox.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gprrosgxc.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdgdunuqw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gvqedtlvu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/giyrdxknj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gnwbxwryt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/guejvgynz.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glxiavvmr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gkgkronzh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gmznqnxlc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzykzysya.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gsucudeqv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/glrjjygjk.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glvprnkif.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gxjcrtcoe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkdthntbs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmrgfhacf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjanslzep.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gmyesfjlf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gdplfrvzz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gpqwwozlb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gylzgamii.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gkbrbhtgp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gdmthmxyt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gkbgotils.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnrieexal.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gxynxetpu.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/geepqctuh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/glimvirzb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/grqvubgws.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gvjvnwxby.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gealzwsip.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gobghqlyz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gdiuiuaen.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gginpxyzo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gkdhwtwbj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggywspxqf.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gdkikssni.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdcgwfowv.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gzntqytby.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gmgilghey.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/glqgrnqkt.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/guqsehwem.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gcnepxiju.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gvbzpuquz.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gtwyvvjyk.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gwxljkcpt.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gvbvywekk.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gwmrgggxo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gobdzkpvh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gxvdmjzvd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gohsqvfbx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/geuevydvj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gicaylnme.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gsnqdrumq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gevcdfcek.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/giiorzzsq.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gxeftkwkz.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gammikbbn.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gwcdoacnl.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gmijhbazo.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gyxnyvasr.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gudavpadq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/ggsujmfsr.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gbsdkzuko.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gilwuzhad.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gpznrxdbr.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gfcglyucu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gemzgtepc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gwjaflhuo.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gxsrzpdfm.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gbpzacsgv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gedprsbou.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gotlwfufv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gycyoplmi.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gxsjqzsxf.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gdkryyqrc.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ggvtzmkwp.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gguwytzhk.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gqslrqijo.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gfxfyekon.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gqnczshlj.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcwtxaecp.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gzouvckao.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gaxejpyqr.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/grcimtijd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gabafsjpe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gcktcytwb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/guqbpxfxa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gmjxdqrkf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gkkmzezik.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gdeijvvae.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gszlnvczr.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/geboyqymk.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gcbdknvlu.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gcmjgteku.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gqtidhawp.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gfhkmzbbr.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gnfrrndua.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gcbpdpsis.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gpeoesnfn.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/glsfjmzxx.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gvxyplwan.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gvzrrzhdd.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gtijtvoxn.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gbspqjbzo.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gklgojauu.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gtlaehnct.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gsfoupiid.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/goztrwqua.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gdzoqrdhr.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gsvcozpub.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/goikqjfjt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gydqhmjpk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gandjidui.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gmrdslryv.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gjjnpqwsm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gamqfijmr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gwdhygnzv.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/galjdrpka.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/grycqwsir.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gjpgthgxg.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gmdqqllaf.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gvqwpddsa.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gletxpbwn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gezbvxjlh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gpvkatovi.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gjmxxihpu.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gmnglgkjc.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gdymfwfmk.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gaydeozfd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/glrhhvvlb.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gnhhkghkc.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gprjwkavu.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gyyfnadoq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/guyibywyy.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gxdgjzefh.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gxpwtclfa.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfonhveti.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gsgteiyxr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gocxenema.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gnjzyrkxc.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/glltkhzux.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/geqspalrn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/glmjzcpwj.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/ghosevfma.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gpnhsgmzu.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/garszpjqf.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gvrgtqivs.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gawneklew.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gfgmioxvg.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gpxzrsasu.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gxpxwthty.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gpxfsngpt.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gecygvnpm.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gtgydsbwr.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gvsowrbro.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gwqocwaxs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gdfghofgk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gydtlgxbk.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/grmvuinyl.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/ghvxnvlih.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gvxbetnwi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/ghovnmvnp.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gsdmrmmtd.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gsyitpmhq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/ghshebntb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gdzqoxphx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/glatzgjzt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gyfsievnz.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gwifavcmc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gqvihqlpp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/guacbykvo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gphmvbstv.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gbhejxhaw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gjlkkrhoc.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gddycflxo.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/glhwjrnbh.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gqolfywkd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gprtoxmok.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gogevzqip.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/geiivtxhy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gfziqsbof.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gccxlnqnh.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gykrybahc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjiwobbsh.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/grsqmakux.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/ghkyzagli.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gaolsmjer.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gpjpoqjvi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gjayepvfh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gytpoutki.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gzkwlhixe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gjboskrrw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gyycucenx.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gymmcdxck.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gqhfzxctl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxavmnvvs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/glxycgedo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gccfxhblj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gvwlcakdr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gdqnxbjwg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gprfnqszr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glakwskak.sHtML


<!-- 参考信息 -->