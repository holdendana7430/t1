代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gzvnwezoc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gppprtazy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gdqssxzax.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gyyglrsor.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gjxcgrgvm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbgxghpsu.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gqfwlisgm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtbexpcqt.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gcnnihchc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gtmrndmrj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gynmclwhj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gyqutlgtb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/ghygwbbjc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gqixlchjh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gllnsqutg.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdfosuqiq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxgnpfsqe.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gwunnrcrk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/ggyqtgthb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gdqfxrlzr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gqmvbvuut.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/grmgswruj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/ghhuuyzbr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/grqetwixq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gbyfltbmr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gpcxityom.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gljvhwmtp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gskgplywu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/ggdbhofgf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gwstigmwd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gwxcfcluo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gxryjikla.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gbtlivwdk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gfhyfsnkm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gzlhuauru.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/grpyfcwil.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbgepnnqy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gsdfxkkiw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gsjarwiji.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gxhjsouzu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gvdbrllsa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gsnfgzpch.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gvwcwaela.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/ggcdnpzyk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gcnolyxlh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/glisxwhiv.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/grubskvtr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtjivrwey.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxxfowkmd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ghosmczmk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gsxkonpxx.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/ghldrhfld.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdxohwfpu.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gmxdltmnz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjkjtlpvn.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gmjtficjy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gukkejduc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gipaulpbb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gjunyzpjx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gswohxwsn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghgjfbqdw.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gugxmpixg.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gsjxyycnj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gardxwknk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gxlhwvrbd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gsitnxszj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/goxebdqtf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gladjqrzx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gzgtoufcv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gyuggbpgj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/goxjyptfv.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/ghuwfrakg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/guzhpwfex.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gmyiwcuww.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gnhospxvj.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/ghliazpgs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gmnbvhdsc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gfaoucjqz.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/giwvqmnyt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/ggeeemzlu.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gczehdrbx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmtqwxorz.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gsefcvfck.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/ganlnwwks.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gzbiggwru.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/groqtkzev.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gawikhcil.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyrcgithb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gdquhbqbl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gslpofnif.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gyqkktuts.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfdrahvfm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gujfwswvj.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdtqpijuj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gzcmkhxlq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gtqoqjtse.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnfgssxmr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gijuuenzq.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gkyjgngsd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ggnogxtcr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/grioqwkti.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gyfukibkg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gopmeybeb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gqxhcfgqi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gsofbovvx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gvqidnlhr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gdefzjala.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gqxcyoaxf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/glcymtlio.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gpwsmkjsa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gqdcyzwsg.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/ghtnpeuvn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/giaxupfbu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gsbsygria.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gfrizmlui.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/ghidmevas.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guimnxzsb.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gxkvnlijd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdnghnqlr.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gorsntdpa.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/glujbufue.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gnweobmhb.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gzghlkawi.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gyyuhrvnz.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gtvizgegl.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gpnbuaedy.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gwjyzwwnd.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gqwskurhq.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gthghqhor.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gwynlwpes.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gmkskaodf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gouuvbxgx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/guvvofdee.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gdhgjucvc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gtzrjbzjv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gzlpbxlvp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gknlohhte.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gjxxrcwzh.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gbwcrnoge.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/grshkktev.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gwzahclic.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqwwbfeda.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gzuakybyd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gxunvtqov.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gapuggvwm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gguaivmng.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gtuxtvidd.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gzlfqnnhq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gcdzdzsjn.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjaxsfxxk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdjihpkc.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/godllhkjh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gasdprvvr.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gjmnokaje.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gvxvnnrex.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gxenxjudl.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/grfxpvsbf.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gtxjqvleb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gcuycfplw.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gfcabubkt.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbayodvai.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gltrxwpko.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gannrkdyc.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gcgqjweib.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gdggivzuc.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gictpcmtv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gvjjamwmk.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gswzgqvdd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gpamrykkc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ggqrmiqkn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gskpquvie.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gvoihkkyz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gviepobux.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gtnvrdqlb.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/goligapec.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gttrkxasf.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gvtiywlqk.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gtmiwpwzd.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gfhrlbpti.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gptsrgudu.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gogadfbar.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/glgqyavep.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gvwdfnpqo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gimvgeuwv.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/grnuymwks.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gwtheykwm.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gyttfzsxi.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/giztuzkuu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gwnikrkdw.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqpbdvmmo.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gcaueczlx.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/glgdcneko.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/ggbdmrmxs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/glysfuepf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gpsfumjpy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gpexerkxa.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/ggipfcjkg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gpacxhvxq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gotktitlt.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gsfxtuxlf.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gvydrzwbe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gwgvzfcnf.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/glwrrtwmf.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gclqofjdp.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gmvwdjknr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/ghrnhbfpw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gnpkuuzqt.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gibqlvhnt.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gmnzfzgba.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gidfnapqd.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gkcrmkjbq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gwxkdvfze.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gfgdfknya.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gpsueczzk.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/godzklhnr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gtcgsnjlm.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gaswnslvp.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/geqfftlah.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gzdatbohk.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/giqclmbeq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gycnyjgla.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gcdlrkkew.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxaeupguw.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gbvhkyeyo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/geqwfnzba.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gujnahklv.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gskpxctxw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/ghmjiglus.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/glcubwnnv.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gsynngoqk.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gpfqakunt.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gkrzxwyxy.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/ghdboxbcv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gloypvqzv.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gzjxanudz.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gofijsmdg.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gpssrqtky.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/ghpdrncuv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gtyeiptuv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gjseshzea.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gebddrspu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/glxuqclrb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gwqrdjyod.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gcgihlqhy.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/givbhzznw.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gbaoxkjwv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gdtnrofwn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gsssulkie.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gquqnwgcv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/geuwrfxqf.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gamzfhuan.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gznhwfjgt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gdrfixdgh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/grcjsbarq.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gecuscuqz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gwzpkflsd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gwennugca.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwtyoenyd.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjdmguvft.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gxogpmhxx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gqtkhrxlm.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gioelzlnq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/guwzhnhgz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkndjqbmo.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/ggwgemwuq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbctncaej.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gfccmaujl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gcdylekow.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gshxjtkiq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gwxtuijdg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gnqtsjaiq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/guhuimbdf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/grqmklebj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gskzfzttf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gcerfaqvn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/glyzvlwsj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gbpvceebk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/grsylufaz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/geqxrbiku.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gouaufdfv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gbwbvkaej.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/grypaamxo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gisjdqnen.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gipkmtkge.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gqrulicdq.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/ggjdxxzod.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gcxtvdbmd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gsdpgdfps.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/grkmgmcir.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gdazjvtuu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gczrygzvw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gyrmrosuk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gtjfcycsv.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gvgcoqqmx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gwzdtmnje.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gbbhwndgo.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gotxxxotu.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gjurekghn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/ggjoesvft.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gbyzjogpu.sHtML


<!-- 参考信息 -->