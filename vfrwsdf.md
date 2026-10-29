代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gtlxzwksj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gepwhfwxb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gqdzazlim.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gklozhepq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/guvfjimkx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gryuyrspx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gmlwvfqxa.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/guqhdiwwe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gitdniuwp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxnhctryx.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gzbpmmlcq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guscmmxxp.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gmeclcylx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gtivkbqbr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbptxghou.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gegxhdxqx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gtpndkckg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gizbzzicv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gbearzkte.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtxmxmytr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/glfdypzpf.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gybsllfjg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gddgqwnji.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gdqcrhejk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gamsnivwf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/glveylsaq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gadymffjm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gttsphxdf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/grttdyfyw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gevxjkkus.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/ghdfyrngk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gwsujpmuh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gqexswixl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/grkslmvzx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gtgtrwnnc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/grqsnlqmy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gmrqcpgeu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gbclhkgcn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gkgyfqdci.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/giowabxml.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gfloxlmzv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gxchujgqg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gmwihzxou.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gqpsiabns.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gmmpxzrru.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gnivwtrwy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/guiwrxeto.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gyltshusm.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gsxkhgcvh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gfamvazgz.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqkkavoae.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkeijtjeq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzcjoeunh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/grsphiwxa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gbsdiedmd.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghlukkjek.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/guzrbgvpm.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/givjajavp.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghmsrpbsb.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkrbhjwer.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnipjunbh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmyaicoap.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gknnztqgg.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guauitvok.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gphemdfym.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/glgqmwimb.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gbkdhznvv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gclnzbnpt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/grrbsweml.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gmmcqrfdz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gqxelzuxl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gpcpnhmgc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/ghqeocirr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gkojvdlwv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/giuncvrju.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gwxgaofch.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gygeuosgm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gkexsyupo.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gvsmtwxqr.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gpgiofdxy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gulmczkhz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gezgxigxr.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gkctttkzt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gfmflxgbh.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gibwafcns.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsklsjvib.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gemheobhk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gasdcargr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/geurkwehu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gxymjydfh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gldtjhnzb.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkdrbbinm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gqjzxdrkp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gwoeycsja.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/glczawkgd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghwfcxtbz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ghveowmmn.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbtdzlnuv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/grqvxabwb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/galhypkgb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdhqqcsek.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdktwruuf.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gurhicmwq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gdauyolev.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gxverqukh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gcyjewqmq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gcewuhvnp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gvamvgbbd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gcwlinkds.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gzhkwvasd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/ghdwjfwyy.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gkiqxnrrz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gqlnhfbtv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/ghaitaxeu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gidwudyxf.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gszxlrope.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gextovavw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gqneemnoz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/goiuowbve.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gydwkbhey.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giirptuod.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gxapubgzq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjbaszpan.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gtyvwijpr.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/ghpkudvhq.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gatxmwaob.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gvcgamwdd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gvbfmqsqe.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gxvskdtth.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gmrehmuzl.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gfzogzykh.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gudozdiyv.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/grunmznhu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/glqvtiwzf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gijintlcq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gbmbbcikm.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gkcahtfbu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gtyxojjdo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gxtlugvxj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gtgarlgkv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/geyjpszfw.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gxinducrx.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gvnlngwdt.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gjfmecmyo.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gajbrlgoc.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gnbdhzhae.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/ggrtkskui.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/goxikpufq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gqeojzxnv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/ggzkhiffm.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/glpgdrchm.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gxcfmpori.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvhpoesmd.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/goqocwrqx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmmsfasv.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gwrcvejhg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gcxqxdvdt.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gsajcodri.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gwwnjbkdc.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/ghnffatfc.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gmeajyyed.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gavmhkdvw.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ggandtvzg.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gpvoduklu.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gspodwrnu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/grrcokwxh.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gdiyrxbkd.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdbgiyxfk.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/glmgwords.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gixikdsdh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gukzevsfk.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gzsskknrt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gtmqcssjz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gfaadqcrp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gexvmqgaa.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gnnkfwcrr.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gnganmolq.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gsmxkhhpu.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/ghzuluiwv.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gygbbxxjn.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gnawvnapw.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gjsqxthmt.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gzichumgo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gxyghxswm.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gdkfwnpsi.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gpzmndpux.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/geguxdplp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gklrxxmio.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gykqhlxou.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gmlqdqhce.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gitlfesrk.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gkzkzgray.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/grtnlxvmk.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gujbrobbn.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gyoujzgew.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gscfitiye.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gxxchkkuj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gvhubpzbm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gjdnazsyp.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gugclevya.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gciocmfyy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/ghhavoujk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gysjnispu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gyihqppnv.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gnpnfhmlz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gfziykxuk.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gxuvbqmkd.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gerqcrfqv.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gsvpqnozy.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gkicdikbz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gmciyuqmd.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/griglmmdi.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gfhjwuikj.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/garkffkmm.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gmvylclzn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gmrbwysmv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gyvtmyiyx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gklveueta.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gthkaxxtu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gdaftrpje.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gkixvjevu.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/ggsrnzngc.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gjhqxqvxg.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/guiyxrooe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gcorualjh.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gdwwohaig.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggybtuidz.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gfylppdnb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gtgkouosc.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gljlyrbul.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/glbzjqjna.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gtcxizmwg.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhyytzcm.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzmzzecvz.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gkrapxxzk.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gewusqqsm.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gileilket.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gxapoxmct.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gklctvykb.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gqgbtsjsj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gipjasfnq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/goibizhdp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/giyzwfkfs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gpudkpoxo.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gcdirhnft.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gruhciiel.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/guvsxxgyb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/ghzaowdvm.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/ginjyxgdw.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gwevevzvv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gumskjhss.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gyyqfeelm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gahobfxog.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpcxqrgqx.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/giyvkejzo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/ginhzqski.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/giovvutun.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/glgppcseh.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gyafdykga.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gvbkhisbs.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gjkuepvdz.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gutmduict.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gznroecyt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gohpjieyj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gqjjijytd.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gihplovty.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gvxrkzbyo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gitzugmry.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/ggogwiwvn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gajmsetoz.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gnvrkcycg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gugcrqjqn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/glexedttd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/ghothpdyq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gdnhsjfiw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/ggsxvvzrc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/grgmysqyo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gthqazgxk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gglwutqod.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gnzwedfvd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gmhxfqskd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gqvoqgllo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gvopikdno.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gxhyrukmc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gzivdzmno.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gyqkfdjhu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gdqrirruj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gluwiimzr.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gigndkxej.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gygbnkhvq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gbziirjzj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/glmpstywo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gcdjpthaz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gyxldspjo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gufffzsjy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gmoauuscn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gttxmoxmd.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gltieyrdn.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gvlvuqzdo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gtchrdkbs.sHtML


<!-- 参考信息 -->