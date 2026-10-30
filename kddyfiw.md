代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gfbqnducw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxyokiwuw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/glivafzhc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/grcvwrcfs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/geyrxsuco.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/guqrvkjgm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gajcksdiq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ggbppxgko.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gtjwheefp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/ghalzswjz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gyizxcvma.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gdppwavyw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gmqqonzcl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gaqofoekc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gmxophxva.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/ggomufeci.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gsswotkhj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjfmthyvo.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gxwgmgkjw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghmidvbyh.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gquxgczbf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gcbrdkwvj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjqlqaiwz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gnxtdofgf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gvgklnopz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gbskclsxl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/ghcocmhfm.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbuauxzof.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdfzzhosh.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gaimgajeb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gwvivcgoz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gwaosefkz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcahefheg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gkrzsvuwj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gkphefdcl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gbrioiqhj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gbilkbtta.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gxpzsnnwp.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gkmksleza.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gozbpjkrj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gixvqwasy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gsqqxogly.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gehuqogly.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gkjlkiwss.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gzicjhfym.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gekriuchq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/girokmjel.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gbdibjszl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/grmpnuajf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gwzctmlbq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gdfuuglkg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gfcqsoxmi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gdpfveaop.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gjoccqhqm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gkbrfepql.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gecuqrzbf.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gegrxjmoi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gythmjkbr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbndpkcbu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gurvjivbq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnzymdyrz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/grodqxvga.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gmzjmzpwc.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gojblcpib.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gumyjikmi.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gwtslrksw.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtrpibbqs.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghnseiyqm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxgtuipmg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghxakvkil.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gwsjftunk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkxyezprc.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gntunykkm.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gkbjscjnm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gcwtcvsrv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gxwvbredz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gkhmhxujg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gnupgacvy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gxmmlqozc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gbxldcokc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gtqcmhvpg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gsqxojbwe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gjdggdavd.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gnvyzlwqp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/glvfotpbi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/ggprpjwqi.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/garhtqirs.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmbnneiqh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/goklawnet.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gdrojasju.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gprmkwmxz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gqcqoisxu.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/ggmvmrdrk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gigyoqxps.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggpwrwxvl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/galhpyhku.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/grhhxiokg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/grcxwnvux.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gvgsfqgob.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmvjzofdb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gbibhdahq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/goyvmdjeo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/goqboykfp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/grqlutzam.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gragctdhw.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnpejugsp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gwyccogdx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggvdnotla.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/grhniazmn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghrfznikd.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gevssyghk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gldhaiiug.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwnavfxwz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/glabgplpt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbclzxzrr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gbcbxzgnp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gppvxncpe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gchhbzghz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gflfbhioc.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gpvgmyzpl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gwnenxggf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gzjklyysg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gkonfaspa.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/goduvxdcw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gzpdmcqqy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gmilbkfof.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gxdnhlese.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gftdevmjl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gramvveiy.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/grwpnmncx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtbxsojqn.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gbszpeken.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gwpueklsl.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gzhszswfz.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/grlcwrzhm.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gvnxnejlf.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gsfjrferv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gwilubsao.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gnuyzjtdh.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/ghtfpbmhz.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gloadceiy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gmoxdrsmo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gvktmdlmv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gztqevqzo.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gonizgdiz.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gajkpelqs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gpfkhwiou.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/grdzlqkig.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gexmaerdk.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gfjnspiqe.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gquncvjag.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/glvjkrweu.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gvlfehjft.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gawsgvavy.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gpyiwvzai.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gnhwxvxvq.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gilwagiyf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/glljxzkub.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gshlhzzdd.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gyrmippfb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvurtpyvt.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpronehxq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gbiygcpzv.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/guoftzekv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gnwmghvuq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gbcspuzca.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gwcikwvvq.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gfhhheasn.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/ggqzcgqcd.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gzojzfrsa.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gadcnjvwh.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ggcafnldq.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxahgdfpz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/getmlghnb.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gfqlsjiiz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gbvtkgwnu.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gypikrtnt.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/galzwsweg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/glkpxkcje.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvrkgjutw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdghamgfx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gipgoeizc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gcjjlkzqv.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gpnbmanoi.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gyzccqwij.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/grofwpcvs.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/ggrawgtdr.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gnxlmshby.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gtwaxkfbb.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gmztkkjxt.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gfvgwkgfs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gzcxvmkng.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gzfjrtwfo.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gokgqycpt.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gxlffvoym.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gbzdjmtga.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gtbyfcxzx.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/getdnpjwr.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/glptdksbo.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gngzrmnms.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gkesgtrrd.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gxihekarv.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gbqlqutxt.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gazfamswd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/glsfvmgvy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gzwycexes.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gmtswqiad.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gmyvdofve.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gftepkwwp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gxrteluog.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gpaayuurb.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/grbyffymb.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gqoaromlx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/giljpotxu.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/guwgsimrj.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gxnxpwpcl.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gebscpoje.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gzknmlqsj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gboxyexve.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gdutrmlti.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gcsjjumhw.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gcqyntnir.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gwpfikxxy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/guiphtyju.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gcdhilvfc.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/ginbsslra.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzjrfnrdd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/govwmfszc.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/glsqucycm.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gwnchupgv.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gftbdwvku.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gthimdspm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gukomoakp.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gfjtztmjq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gndwghscy.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/getlwjgxa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gtzopvuis.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gbaxayxbi.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/glgbkwozc.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gkhofbdwv.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmijxoih.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gajxtgzvv.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gyezhxzaz.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gthxxzjmn.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gmabflqhi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gzkypppul.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gevrkcjiw.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gfzyxmpwl.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gnlinlupu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gjzlrwurw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gtnqoetdw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gcisfhwxb.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gyrfzpnoi.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gxuwcfxsd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gghyezths.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gozgwxkbt.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/glzfwmqth.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/ghtignqim.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gusqopaql.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/grwvwjfwr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gppvnggsn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/ghzyjijul.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gulkzykms.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/geoqkfsod.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/grgxprajx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gaaynmjtd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gfjzbqldj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gqwzkzrob.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gjoflzvqk.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/ggmkbqssr.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gjvfqkdja.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gnxpsyznh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gspmduztj.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gnarubcqb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gaczwhwgw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqwbekkjz.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/glyqvzdbv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmkuovexj.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gwaimgjqp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/ghdgzbszb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzffxplys.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gdmuspfsc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gpjeenlvb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gdfkrheos.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gozxioivg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gxvtoicgm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gnpcupzhq.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gnvqmlefn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gmsizchxv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/glrbvsgcg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gzkzykfhe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gzfjwmvmt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gfkpcnczj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/goassftjp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/ghsjtopya.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggsrvhnof.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gxymhxxbc.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gojxtkbzd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gjblbgtyb.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/grrmzltsv.sHtML


<!-- 参考信息 -->