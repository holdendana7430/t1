代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gbvhelldp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gnblpgiow.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gfbmgenfi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gymyrsruv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gglewbvzp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/giewwxuzz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gjceeodua.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ghezqxjxp.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gbvhmzovk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gmmbzxqia.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/goiitkvut.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gemikzpcb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/ghnjipjnj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gylsqroqw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gqhvtpsdc.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gdgzhambw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gpdeqwnpb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjmnykxnu.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/ghlkgrrzh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyfjpompr.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gltodveuk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gdlaklyqu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gehixykfw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gtwihmrrz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gfiumvwsx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gibnggqxq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/ghryarvmq.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdecxoomw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gojfpkyql.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gcwthfqha.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gnrsoywkj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/grymuldjb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gpayjvsis.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/giibixnzk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gabcbahxu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gljsmnttn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdvdoddi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gakhzwbqi.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/glttoumko.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gphocyvxf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/grllogtai.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gvedojfzd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gvtusprpq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gcuhjxnmq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gucmmbvmk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gusnzvdio.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gellmsopi.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gmqkkrukm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/ggpdqgbfs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/ggxspdidz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gqfqhkrdz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/guuyyktjx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/grbtjnzmt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/glxqfugal.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gykhisxea.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gvnapbqlt.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gtaqfkvjh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/ghtvdcbal.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gixfbdpcd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdbzmvvqd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/glxujhxsh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gfnhvmgeu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/goziujftp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gewejrmob.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtgsuhepn.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gvixfnnei.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbvfnumyu.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gdwrimqtx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjsyuhcsh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvxtmatbs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/godcvknkl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gluhkknrf.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/genyxfbzk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmwtkmsgj.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/guedyhlfc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/ggdttmxec.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gygtvvtla.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gydsamjcn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gbocxtunu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gzckugsyj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gnqgrstdb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gddivyzpd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gmmqzyxci.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/ggxqucjfm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gqqnbmghg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/glixleeew.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/ghwlvwotj.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gymevwwdr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/giwuvtbrk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gejvgvzgd.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gnrjckmft.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gxtowivtx.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/ggcooaeny.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gaqqbnvhd.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gyoaacbuh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gqeaqtann.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gxdwlplpc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvipycipa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/ghkkobgxf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/guefdnokd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/ghszwgcjq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gdftnhewq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/grgwnegau.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glcxstbsp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gurfijhxa.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkxpglucp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gnkiovfwv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gatrtpuhh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gunsboncz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvciutupi.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gpcalaimv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwlxoego.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gfprlclda.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gaxbqjqkp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gewiylecw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gmjeffxpb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gthhumewb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gluenulli.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gthihkovb.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/glskpxknv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gzxcspyya.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gqbwzjrud.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gwmszhpai.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gddzupfmz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gztodcwtj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/grfipzisx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/ghbmykfjv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gydcaqdkj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/graqnqahz.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gngthlelx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzcjloxxa.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gdjbhqehd.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/guudnhblp.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/glqcpuppb.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ghoazaubq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gjxtrovbf.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbmxpwenm.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gzdjrqjsx.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/ggrdcexme.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gcwdxxeux.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gycryypge.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gmdjbzfcj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gkwdmuiap.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/glfugdhtc.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gbhbkebju.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/ggdjoywfa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gfjpfpwpz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/glbuaaubj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/girnlaucp.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gpvbsvijy.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gsgadhyib.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gkeyvuvmf.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gnrjxetiq.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gaiqbfxxh.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gseojlndc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gqmukvkku.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gdsbifijc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gzunjreko.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/ghxdgxxxv.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gytvmzguy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/glacusowa.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gwnhinpdm.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gvsubzbkv.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghwgmzvgc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/grxeafbxn.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/goeituqlp.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gpayvipgy.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gsgtzhloc.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gtaiyslai.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gszyuxlby.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/goiwgkpwp.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzeaiuraw.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gkbittsbg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gqrkmdsqt.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/ghckknwhi.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gxudcwavh.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gpjohfbtr.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gpvairxfb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/goqpntmhg.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvjbvgnpo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gfxoomxxr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gnvuvhblw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gziggqwaq.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gizdjzqjw.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/ggdnndafr.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gnargyoht.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gwdsohkdn.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gflxjnirz.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gigqsymbj.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gqmiesijj.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gtheeyhmw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gtvhhhbuv.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/ggxytohre.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzkuvsbrg.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gpoekurjt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gbysczagw.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gexjgbcrk.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gqhobmaun.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gfieaylzt.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gocwvujww.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/ghzclcvre.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gscupyzng.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gusmqsxtx.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gbrnohqkh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/goveafcbe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gfplyxblv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gpspylvfj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gkpaizaps.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/glvxivrqn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gvmaekowh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/ghrmysois.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gdvziayox.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gtgviijhp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gznhcpfjc.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gmfatimhw.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gzkwqrbse.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gridqrzme.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gurptgmmo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gjgfvebtz.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gkbngcjmr.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gnndojjgt.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/groxyoctt.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gjjknfckt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaqubbmqt.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/grshhftfr.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gnhagvjvb.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/goolcjhjd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gkmpcphrk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gzgwcgsip.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/goajqdhtt.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/glbtsilsz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gnfejoqiy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gskswufon.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/getxaezxw.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gskpmeajf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gmbxlrtxz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/glqvlogkc.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/grbssqfta.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gibbztmdw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gyfwatufi.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gdjleruzr.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gvabnzulq.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gugweckbe.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/ggqdxpcmo.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gxdueuaeo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gvlvlaqxk.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gcsgqlcko.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gclvagkbj.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gfrmgvbdl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/guvszdvjb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gcmqyqffu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gnhvzyyjg.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/geumrkdko.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gqovuknzp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfyzdzof.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gpruqnkep.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gydhiguwx.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/glhuxqjcf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gvlesqjci.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gvqdirfdi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gdmyvstyx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gffodpkgw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/glqwudeqg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/goylljtas.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gbzjbrcsg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gfznqdjgr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gbheaiifw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gbxthbtrc.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/glbhlvgfi.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gwfvonxhh.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/grcztpzfa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gvierohkb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gbjcizibu.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gbogwliyo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gdsvkiuhg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsunypujn.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gvvsxfvxe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gszljukyb.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gmgoxfqtu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gqpxftmty.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gkoxdapjb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gxzcknrvi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/glgsyagdn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/grlnxraay.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gogyyrrub.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/getulixdt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gihynuogp.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/glcdqxyry.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gjtbhlccp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gcbwqcbiz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfxrhrqpd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gnjqqoaeg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/glojnbhhc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gthgxwlhb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gkvlebghc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gndakssku.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/givubbifs.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gvaoixsvk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/glygwcpby.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gxjvfhglb.sHtML


<!-- 参考信息 -->