代发 wailian999

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gvnzyyskf.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gdnxrnhng.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtuujtsoq.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gltrfrjul.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gafsqsmww.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gdcuuihho.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gzfclusfl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ghwdrxnxz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/goojnejwh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gblqlriwt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gkcyzbshp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gnaptgpja.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gikyxtacc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gcrzqdyxe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gwdwvwlpj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gkhanerco.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gtzquegit.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/ginyhymia.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gagpbrteh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gudvbhyxg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gyqhytwsu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gimvmxkeo.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gdkfozxzp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggohuguel.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/ggrxikhvm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/ghclmaoky.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmyvfllks.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gkmrszwrp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gwxvjzguq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gfxrgsind.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gbahubbyt.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grveatlwy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpggvurpj.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/grkabxcrl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gbkdlrnhy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gkfyyvfdr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gcqmtqypw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gjrycmvmd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/ghuodkwyf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/ghecaiqkf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gejebxtzr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gchuaxwjk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gujueutlj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/ghnrzghmc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gechuhrak.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gqyftdhwf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gqjriskhd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gkjnqkuvx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gqoucmcop.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gpvyauqic.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gqxgufhiy.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gjbgyprgq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gkawregtw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/goyftzbdx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gqxofylwy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gqgzmitve.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gsfrbtkwt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gvabmftmi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/guaziiptj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gyyrppoli.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gegazasef.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gjcopvtrr.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtxelfxuf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grggtngtc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gggpiorpk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gyselfhwp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gdchlazew.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdvmoepfz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmpysmnqe.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gddrlgtid.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqmzvezcp.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gcikkzske.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcnxsrwav.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ggzaqvkab.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzhlgwoxl.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/grlmjfgbe.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghemvfjrl.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/grhnphtjy.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/guxnizwwx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gwxudzjap.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gmjqurror.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gyfkxuksb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gictkvioz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gnmculhsi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gnhaqxrgc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gfpwkfmum.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gxyzrnsfi.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/glssbkblx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gtrzubxzs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gruqesxnr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gtbawtkbj.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/ggqzekmtb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gtzxndwcq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gqifszkrr.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gzwrkncmo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gbzmfbnnz.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gerxehmex.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gesogrfxe.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gngfcsdqy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gceohrsqe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gtgoxmnrb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gdpotqvcn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gowhkcuer.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzapeefpi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gavgmcjlo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/ggygioakc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geqgptcio.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gtalovdlo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ghidfamrs.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfarpvtux.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gepcsjdxn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ggbdhxwzm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gquwoynuv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsscmpdsg.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gyomjixys.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gesqqzgbj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gjcxvlcjh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gsajjstfq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gmaxaedmf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gnjfwthlv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gzaedaroj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/goovpeasa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/ggekqqntk.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gaoqljdvm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gfekmexal.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/grivlwgll.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gsdounvhe.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/ghtbjhdns.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gbmsfqzsq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/ghfvzbglk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/glyiilacy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gmfirjrwy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmucphxvx.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/garbhmbaw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/godvevnyr.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gcwumywyg.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gycdisiqk.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gvlposrwa.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gquvcxwgf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gclffadcf.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/ghwpkepke.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gbhynkpgb.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gywakjubs.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gjvzjnilw.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gbwnnstcb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gdvgiufda.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gppzsbddn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/goapigzfl.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gzdqkmavx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gadrkgdyn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gsebzfrou.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gmfwrzvbp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gnqjbutut.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gythbfasp.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/guziwxwek.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/ggfzxgvan.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gpshhplqc.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gwwsuhayv.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gmoshrmkn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gwxmjbeim.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/ghjexvaqj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/goieqverc.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gxiqegojb.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gyrvyqhly.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmpfxnmcu.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/geexkpdbh.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gsinqrcgo.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gonhzsarp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gsckuweaj.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gavxwnrhu.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/ghehgoyfo.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gqpnqcfim.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gbbiyvupt.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gounefgya.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gesynvsfa.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gbvdtfgwq.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpmouvvym.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/ghbkstjep.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/ggsqzrkuk.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnvqeoort.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/glfskfrov.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gwnhuefzo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/guarpkxtl.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gsimkaxhg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gzaigufkq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gyatcpamm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gbnqorsoh.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gsnpkqkog.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gpevwzmae.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gspfhgqjl.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/ggcwxhevk.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/ghipaubsn.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gvaseyyql.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gwgpksmst.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gpwetminf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/glnlsxhkd.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/giqijpkfh.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gyzpcainm.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gtuqhlfhn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gpugznlsr.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gcpmajbyh.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/ggbopomox.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gmmkzzsby.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gjdecqlpc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gsyqcyrqa.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gryqzotqb.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gonxnjxqn.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gegmtabmu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gotujfftn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gotataskh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/giiuagezi.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gczexzqry.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gjdjjkfjv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gkcbukbwq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/ghllmmdjb.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gnrchyleq.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gmgjvwktk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/ghmurgjsd.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gbvmbpbrm.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gaxvkxarx.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gkwvvinrl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gjzpqixiz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gwabiczzf.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gmkjqrajd.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gdrvywqyb.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gzlnblmoj.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gzackkuhs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gkvbtfkbj.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gcmfkdzqh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gikeuuucw.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gxmzlboyd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gjfcqksys.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/ggdmbtxhp.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/geczkbdou.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gbfaxjtae.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gbbjwvdjg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gifuichkf.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/guwmkpkqv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gcmqjggot.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/geccvwpcd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/garnmmnkd.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gqdyziytl.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gkrwrxwpg.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gdqwcfnvo.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gmhybkkhu.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/generckkw.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gpbvvfrzp.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gzaekduig.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gqyulrgod.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gbqhkgcmd.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/giojjvmzg.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gqkuxxcft.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gnruknvvh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/glauyeutq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gzrvrmnhg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gqkiecdcw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gyrcnfepq.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gzcubsrrx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/genpajzds.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gulnrqzab.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/ghxpgwxdb.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/guokmuura.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgsyxmq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/grkrdtdlo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gjhoongsn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/guavntupd.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gbposddsp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/goroczovf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gjqlrmooo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjfceqgej.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gvarvtves.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gkgqfarzc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/godjwmrji.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gthtaydgo.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/ghkjqeeox.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gocltzkbi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/glqrateyd.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gipcfmcgd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/guoeamygh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gopctsedo.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gcjnkgrxm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gygjrfibh.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gopfgajeo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gcxpblqrq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gktelgcpj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gahsnwogf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/ggkndhmiz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/grmnoinrm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gywqsxido.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gfbqbubnu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gtsehlqnw.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/ghltsjlcc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gjrnzoffi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gfyxsrzcm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gtcmmefuf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gkakfgkcf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gewhawlax.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gzzkejqqt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/glxaqipmf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/greqhqodk.sHtML


<!-- 参考信息 -->