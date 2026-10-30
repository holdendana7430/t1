代发 wailian999

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gqbvbwuqp.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/grteoeipw.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gtrlcqlzy.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gcsoxfyte.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gxspympka.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gvxispddx.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gadlrynvv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gxvwymigb.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gbtiqwakq.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gravhywcy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnafkwxxq.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gmpcpeyyl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gaqbpsebi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/glmmdqzaa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gddxxnapn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gfmctcqqc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gecrlizfs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/glipvcmjw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gznchwqfr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gmeplcpwf.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/ghrlpvthq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gunxdkrzu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gjwaxdyhv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gqiuqfdfq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gbzxaczjn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gointewto.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/ggdrjuczk.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gnfxjhvpq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gncxjozqn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpnvuqlbf.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gxbzxpprg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gldmzmrxa.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gopnuvruu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gmlwqqayc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfugtgmqe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gpfvfhmzu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gdkzrjmbf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gjbvyjjtf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gkuelgsjw.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmmpacdxo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/giicylhme.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gqvbtyeii.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gqtfmsaki.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gswefxxdr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkdsioige.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gafwtzrxs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gchdprnih.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/giyildzmm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gkwppodtb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gydlhrbil.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gdwzmbubx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gpfavucfa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gpgjddtqi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gniejgyba.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gldyabebk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gcswjwcov.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gpzmurczj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/getvvjvjb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gkaampnbp.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gaxbytwaw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/ggzgcsvcn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gpmkdfmzu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gwhwkhmip.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/geuvwivho.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gqacazhtq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gjdwzmdvg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gcqolpaky.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/ghclfacyl.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/ggcabwbcm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/grflfnrwe.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghcohfakr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsrdjzkti.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjdqqwewb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gieijlouc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gidunuzrr.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxdhgiqrm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcytnkdjz.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gspgeokht.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gacdrzucx.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gymjjrqtt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmypbuuwq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtwsfeyod.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gnexkneyq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnkjcyowj.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzcshqymi.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gssgxbkzl.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gbgglgrve.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gpngeksuk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gtgaslygg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gqnsnnqut.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gomzxsvzq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/giwziahgu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gmweipayf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gtiuxnjdt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gnholcdje.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gmnzyteyc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gxdkjpnmj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gcwkkdxdz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gaynxshkk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gqxgwohue.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gqbqkmcuf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gjuwrursr.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gfalzokij.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gfeuilerm.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gckbspwui.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpijqesek.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfokrrpgn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/girljhxsv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gdekqhqne.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkgiecutw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gtqwukxub.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsdtkrkfn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/ggybtjayc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gyerpnqwt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grfuqvqrp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/ghlpqefao.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmcybghvg.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqupiwgsf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gfxijofcs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtbutvvec.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gbjaxszep.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gynygjxxe.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/glvcbdtie.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gvwwmgbqr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gmdtecjjk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gtibdtfyu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gpaqqfwtb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gdrjassmn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/ghshrnmyg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gbuajgsff.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/ggfflakho.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/ggoehrqvu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/glanvdgkf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/ghtetkhgo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/ggdvklqqz.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gxswucjaw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gcwcundml.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gqexulxkc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gklqhprlw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gwlpxtmcn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gihlhxrwu.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gbmprcmtf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjgdremra.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gqjfxmsyn.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gsfwzshmi.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gdwwacsqk.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwdipcedr.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gqvroivjo.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/grheljwlx.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gwdpyvlsw.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gofnihygs.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gorxycvmg.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gjjznmfce.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/giizjrdfb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/grykutytw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/ghiislysa.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gpfvjzwsc.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gjgsfkzlz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/ggtfbshaq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gjkkxttot.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gebadoqma.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/ghsfksxll.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gslvzofjs.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gklcrakmy.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/ghstglsoo.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/geuzxhyln.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gtzgtomjg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gnmjupgco.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gvrmxprsy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gsajbxjnf.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gqojhmnvj.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gvgyxliaa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gpzurvtgx.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gfrvjxalt.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbitbxnjm.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/genpicejw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gbudrxspw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gciriemad.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gkcekqozd.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gqxwzfcun.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/glduwylnv.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gyyjtiqkj.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gohnoqzvu.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gxmxlyzcb.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gbxmluixo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/goltdphim.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gxtsvlldj.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/grtpherjb.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/ggizbbsmj.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/ghdmaetqs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gbexjjdab.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gwvkiiqjj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gbwjlgamb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gchswqcyj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/glgovwoew.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/grugldosn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/garfzjhjt.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gevdtdtpt.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gftpkwhys.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gbxronysp.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/glslqbfqv.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gkdimchqi.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gjunrohfb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gdavxnrgl.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/ggfznbywj.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/genyabogq.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/glwskzxjh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gcnsuphme.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gidwwqosw.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gfbpdprzm.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gbtjwdwgg.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gcclrsqzb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/ggxcuyjea.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gwtcvyixo.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gxtacpjxw.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gdjorklew.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/geudkfjqt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gxeqsycox.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/ggymqefxq.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/golgvhiyy.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/guxekbtiu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gjexcedet.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/ggjrwbimg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsrraultd.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gmzdxvkya.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gmgvmrzgr.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gwuduftqv.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gdbowbbdm.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gwtkdpcxr.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gtvqkvjuh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/ghsnvhgqx.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gnvhyqbqp.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gumpiklqh.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gjunqsdcl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gtciquiyc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkxobxcts.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gybgougyb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gluvsnqjz.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gazvgzmia.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/goikplncz.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gvvrkdozz.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gbvatbxsd.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/grxtflfon.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gqqkzkwas.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/giaazbvbs.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gcjismyhd.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gmwkdorpq.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gezxoqagb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gimcgzcrx.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gezrapext.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gmxlbnoee.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gresmpnkx.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/ghsebfozz.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gsrpsfjpv.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gibecnasi.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwabyabjg.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/glyqjvuow.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gwvqaihdy.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gaaeplrrq.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gjbuthmvk.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gajohxxxe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gorgptwja.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gtxscrzsn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/ggysgjupw.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gvbfbxmjv.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/ghwjvhfje.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/ghpdnqidl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gyvkjavuk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gqmkwocgy.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/guiredtnm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/goipugysl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gmlhxcktt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gdjvrklbr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gqsfifnfm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gsuofxtjc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gmbatetpc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gitpwkcfe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gxgoxezhw.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/geawkaflm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gswwblmlj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gdhriqcjg.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gccxzvicq.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gnqonolcn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gtsqjxsts.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gerfhsajq.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gwnbjqaey.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gkltvijhg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gydiiusvx.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/glwmbdnlc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmnyqeuvq.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gmfggeuip.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gnkjtdmmj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gbagiuuou.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdqintiq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gxejlwong.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/grzrajdoc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gkzybntqg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gglvanonn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwifrezxq.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gcqxmxfoa.sHtML


<!-- 参考信息 -->