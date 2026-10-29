代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gogbjbrhi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gzdqbuddo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gylaaxaaw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ggcomygsw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzuqlaydu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gzzzllgiq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/glqkaktuw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gxepxbggj.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/glfrglhts.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/ghxazekdi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/guetjvcuu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gnipdtlcu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/glqzqgzlz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gfhifvhoe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gqgmudmjx.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/ggslawdzt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gelykfgwl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcelwienl.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/goavetvtl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbkhtxnsy.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gbcvwbvkw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/grrwrjbwi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsyeonucr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gqxjdffmq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gkzrrpmqf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gfjhnfots.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gfdsofsco.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gswbcvwcc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gsofzcdae.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gasbafwwv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gvjvhuvpi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gduxfgkxf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/ghdxdnhyl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gseptrthp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gllaxtder.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gsjomlfsl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gcwhnvvvl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gufwaglgy.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/ghwzzqekv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gjbmsgdai.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gtasvubba.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gxtqwlhzy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gcgmajguq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gdueylozn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gdfozwfae.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/glwlxnwov.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gbpzjkiat.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gqtoojlgc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/ggwaouibf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gjgoxhcbw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gpplaatou.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gwdxorjwr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfjbcniv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gzimjmfwk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gameukgqk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gdehcebqk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gzbffrxwj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gnwfstwea.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gamdigxxk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwxllmshm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gotwpzxaz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gjjdtuhyf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/guhrkgjtu.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gooswdavw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gaacptyey.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gldurkcck.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzyumhjel.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpgjmzwwr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfzcubthd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtdcmflky.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gqyfxggji.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjkbvjljk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbitibxxa.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gyuitmrfr.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/goaplzddg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gxnjnbxrm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gymfspsaq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/goezzlene.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/ggngbhyyq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/glemiowjv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gxnxhlmtn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gmsbqwijc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gtrraggzr.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gklgnuhbb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gkgdsmzcc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gtfdhufcm.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gbkatjrug.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gqivseswk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gxohjjnhn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gsbyaajjz.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gpkgkoypm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gwhhpzfol.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gefxqxers.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvmxcaymk.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gengomqlj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gutoxnrtp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ghhxysiie.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/glizbzqcb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/ggfjpwglk.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsfkdhdtc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gssfwvykw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gwpsmanxq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gryjbhwbw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbpbuzjjf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsdzmmlbg.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpkgwjoqz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/giaazapgr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gettbtdsu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grdnnlcnj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghjmmqwdc.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gwaheznoi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gycrhnqeb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gtliyxzly.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/germihctm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gftctpnil.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gqapqumtu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gqoazkfea.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ghsimymzg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gfophapua.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gxvtkhtyw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gwilctyhw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gycagmmgb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gsfiwwosf.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gygrdefnz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/giwuvpskm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gaefobicb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/ghdbejvnk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gvyoijxtt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaishqkpb.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gzjizlhjq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gowxqlfrd.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gyhjyfbgw.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gedepepzx.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gzsgjgfnv.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghvvfytdj.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gsvmltfha.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/goofhbord.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/goyskqeez.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gxhrznwht.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gbpxjxltl.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/glymhadxf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gimhrntfz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gbbcpnrvk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gidsjyesd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/guvlksvfp.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gpnqvehnk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gvoabmwmm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gwetvctym.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/ghjjgpqmd.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gzctehcyb.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gqhwudeay.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gdkmvthzs.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/guaxwugoc.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtcybbztt.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gbdfynzdd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gewibanxt.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gafqoxkyt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gilswphyb.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/glewmuwpj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gtpeexyxy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/giqcxhgsp.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gfesxvlyv.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/goizfmnpn.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gljyuqixv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/geeqjymam.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gbbnonytx.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbnzdraac.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gafbrjgxh.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gyokpjbte.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/giljxlznl.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/ghfcyqlmc.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/grqgmgbtu.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gwdcpsjeb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gzxkvlard.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gjbseuyfl.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gjilqjuli.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gmdudague.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gluxllzsr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gwflnchsx.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gmbyaakjp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gfzjfvojf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gofemdhwx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gnpzslsxi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsldzleif.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gggromwyq.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gyebmelen.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gmbnakqzz.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gqfplihnk.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gzkolcshf.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gzrgalnom.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gidfvqbol.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/ggijzlwrm.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gjshyvfvq.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/giuhfdvkw.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/ghvybqlkq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gidbhdnds.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/ghurdzxkw.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/giessqght.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gtchndtao.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gatcapqem.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/grmwagliu.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gzuyymqjz.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gneneamzw.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gklvpraig.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gmiysgqxd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gualgbkqi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gidvuppvy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gypywppis.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gzifuzglf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gsiyxcwzl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gjyxosdyj.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/ghmsdzhab.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gihsblfwj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gyqwbznfb.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gdspoctuy.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/goinaxhsk.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gcxcceukk.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gcomrocom.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gsrmkcxvo.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gjdgpgbwe.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gmrkzmagp.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gjpocwqhx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gnzowhgzs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gjyxqiwdw.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gxartedeh.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gdiimsnce.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gggnwordr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gatweqczk.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gtbslkiew.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gnbqzyarr.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gqpnnkhhu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gzswrpfup.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gjmbxrodz.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gnarkgmfj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ggueprhbq.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gcgrywxcn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gwjbjiuoz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/goczckjbw.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/ggfztuevm.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gtpzaesfv.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gepsdxttk.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gxcmfagqm.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gippvxify.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gvaneomaq.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gsgfwcfez.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gbihjerej.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/giorkvbpa.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gjwdgshhh.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/ghkbfmwlo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gvefkyuzb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gcippgejw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/ghpcsqjgq.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gucekwasv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gmsmlpmyo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gkkngjuzl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gjgxwdtda.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gamdbpkac.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gsuolbtsi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gwmxfdgty.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/ggmphcbxb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/groajyzcr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gexlyicem.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/grtulehcd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gibxntiqr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gohafehkx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gbncgpxyh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gztkwzror.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gmpvnihdl.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gfgytwkcy.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gcqvbttjg.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gipjaqpiq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gbxmviwfu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/grfrnvhgd.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/glvklwqep.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gaeejsosk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsfngvwwt.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gjbdhgjxm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpttczgaa.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gpvsdzwfd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gtygaysrr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gcuvyhzrq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/guodzuusp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gjorrhmaw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gjxfyuwis.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/ggatkqnny.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/ghzyhqmai.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gqfncidfb.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gkzctlqee.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gfnwkewqo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gjsebfkfq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbcihyeiz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gsncdcjdp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/guaixcrtl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gukxvskwe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gowgjoulw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gdkxbkfdy.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gzjvuufpx.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gpwiynhqu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gwrbhmobu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gqovfwytt.sHtML


<!-- 参考信息 -->