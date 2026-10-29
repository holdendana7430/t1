代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gcluetobt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gswlhrwso.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gqatcxbpi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gflvvwawl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/guevfrxdj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gxbtcsend.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gifvouxem.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gvtqqtbmo.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/golowprse.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gdxfloukw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gtywbbyta.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjnhwibkk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gtcogybow.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gvdcfdzmf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gqjrvxavy.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gmpkiajfl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gnqvsvotj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggxwboums.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/glcztueqa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsrnfmvuo.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gzjwilbqf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gzedybbhp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdqzkoeua.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gepemlbab.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gnkiridzi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/ghwpincnx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gzesnhbqf.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gixvlfxun.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnvmtcchf.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gidhkgbuv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gxtmedzyx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/giylcqxpi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gyimvgufx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gdqowpgho.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/grnuhewpg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gklpytcyl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gkzuyvctt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gsopjzubc.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gedrznxeo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/ggwzgyzmp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gexpwmjhs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gbnzfhzmu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gquingteo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gkjfxvfdu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gquydfgrw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/ghuzbpdmj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gamzgihmy.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/glmltfcfg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/guwpvxsdj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gutvpqmml.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gycjhwjrx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ggaikfovn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gwinozird.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/goaihstxu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/ggqelbrwk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/grsbkkuup.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gvkkrsnot.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gjgnbmmay.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/getxfpkkz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkuuqnyrh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guikvfjhe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gphszurdt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gqblhetqu.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnxzyfcvn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gditxhyld.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gtwgrwjjt.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/guwtwbcyq.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnyloytqq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxnzsnptf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsavhnrcd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gazpjgbqr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbnuxhdxt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glocrlkzt.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gpdebouda.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gkkwhgwjx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gqcfthhdw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gzdcilvtd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gxvjtyewh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gnsbgrcqf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gcbgtczjl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gasujfahj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gkfttqhpj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gwyfeuhpm.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gptwjnocc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gmmbbmefd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/glhxivxfl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gudegbwua.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gsqromomy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gurxeawug.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gbzhiahjx.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gbaevkpnt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/ggkagtopf.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/goaloqrps.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghwluuzuh.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwvkodlio.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gdycnkzqs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gjzsctpux.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvxrkzibh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gmqxemlhf.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfhcxjhbi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/ghcabfbuc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/ggjhxmxrw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxlcsspuo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/giymanpho.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gozcocokn.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzcfvwlvv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gqzjqbqne.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gcseuznwq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gozokpncf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gxwxbkryg.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gcygelprn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gaexxciza.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpqtnxjiv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gvmgzyugr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqwmkzdcw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gdsbrbpzz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gzeutjoov.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmbpctyvp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gaachhkwc.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gybpurvci.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gebjlbyyl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gxxpoyivk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/grejkdkdj.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gulgjrvyp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gnytydlhd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gsramgrxq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gdkkioejh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gevfrjsjf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbwzrllxc.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/grxzyvjog.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtpvcwwhm.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gyejeredw.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gvvxjelkb.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gucjukrwt.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/golqezwbm.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gkkheqfqk.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/grurhcneq.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gfllxgytc.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/grpivuzbn.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gpabyjpae.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gyewncsfk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gcsvgeylv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gpztxdizy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/grvfxyira.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gmzdplsxr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gkiqvtytv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gewnhelzb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/guibrnrvv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gqncodtds.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/glpiltkmi.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gkprtdxqu.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gisauokia.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gsytccsxj.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/goivsqzyq.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gvdksatgf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gzjbajcer.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gzkwdbgyl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gpivxjqrv.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gdcwgiwun.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gvjxsgmjv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gunxmrywy.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gzcpsfplv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnlkkbwf.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gycvemnlo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gbbbndjqe.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gczlkdgkx.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gvjsqepfv.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/goqxpizzv.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gwhzbpbqi.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gdbzkhyaw.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ghyslfave.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/grqwhdfxc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gydtfjcqt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gqhdmmadg.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gaoyivqxl.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/ggdaglkjw.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gikewnvmp.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gorygwyvg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtybfspav.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gluapqvlt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/goahrbqky.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gzomqzedn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gzvpxvbxf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gqoxganvr.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/glrwzlsvj.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gghsmbbcq.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gijoctrjt.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gxjaoocxz.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gvcrqtody.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gmvyziski.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gvomnbrrg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gzfnjibut.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gsbjqppdx.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gmugbzqnx.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gfmrxuxwf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gxcsyzfov.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/grpjjlonz.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gmqcnuwez.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/ggdpcvgck.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gdtiqjdse.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gtzdgfxnk.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gjhqinuvy.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gcgljjcso.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gkeooklqv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gsmaprlbu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gdaybaiyi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gdrvfatzm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gfocdqqbk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/glqaqqqtr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gojekzaxo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gqppfgrme.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gxuklkosg.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gfblvbyme.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gvauygnqm.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gbhiiwbsm.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gokknprlo.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gtbabycgm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gmjxilkcc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gddktopjx.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gsboqgfpx.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/giruwmjqf.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gyupogxca.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/ggjywgeeu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gintcjlye.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gmwjfwowd.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gbxinjcdl.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gyokpqovy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gaqefwofr.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gmnxdfagq.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/ghltifvcs.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gefhalmoi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gvexvzate.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gnlmefklk.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaesatmxj.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvxyfhnup.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/golcutvvp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/glsmdapfh.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/ggbkajqui.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gilwjxllr.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gcubxlnrd.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gulklwjmq.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ggfvmsogp.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gqgaoliqz.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gxrdjjtgr.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmrdpgytj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gkdtadwlp.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gkwxireoa.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gdmnmrzlg.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gyafogbzq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/ggwfoafgt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gvonbwuny.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gtlvhemgx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/griaxfvqo.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gstgjursf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gstvewpdb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/glcdpciwe.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gsserseyw.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gvbwdxxgk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gpuuntqgz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/grqwtbdaz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/ggdpibtbd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gfbmgqbpq.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/ghpphniii.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gwdjxydpm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gofxbxvao.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/ghqldximg.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gqfcynahu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gswowvwcr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gpzcwbedg.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gftwehuxu.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gpvuyzdgn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gcthuxqyt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/ghpxvzyhe.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gomcekvig.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gzeykzutq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/girepsclo.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gzxohhmiu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkapmeuhw.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gizzscmwd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/glnyymmde.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/giihobwrc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gqwaabvre.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ghnpqddhy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gkuarbuyh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gteebipcs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gczrprlli.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gcjnnqdch.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gywikcdhb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gjmegqiqv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gsoohppbi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gainhhlfv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gsssxfxmx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gbyanfjli.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gscgjabyu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gjamyaedo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gzpuggrjz.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/giziowlxk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gsvswcnju.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gtrczhrsq.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gylyuevzc.sHtML


<!-- 参考信息 -->