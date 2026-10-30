代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gwiyzwour.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggbidwafq.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/ggjqixogn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdjjplwah.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/ggrhfagun.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gyambydqv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gyicgovpo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gagdhtngw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ggbzqeeip.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gpzlnisng.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gtzvabvrb.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfcunclua.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvvdctfav.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gddnfsfng.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gdnuozusx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gxpltshan.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gbmeolcjk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/ghdvbsfti.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gbgnsuvgw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gpgszhokn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gtykzdjjf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gunenorhe.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gqvkwpuap.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gmpuurhew.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gvimhfrhr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gkazlfvsk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gojstivip.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gfmrwphvv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gboroeelu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gkeuvdjwh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/grnpfeseq.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gkkxseiwn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gjgrfyefc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gjimzqeak.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gefxlkvjs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gnidygmfl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gzuqawbmo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gsuzrfide.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gxxqjzchi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gkeacmjeq.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gfneubkfc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/ggsjoikmb.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzbtsesxx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gszdnhpvz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxfadxvnb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gswcahexl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gemthkspf.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/goxvpprej.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gftiudxdz.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/glknphpef.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/glpddoycw.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvbglsfut.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqfoekucq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcguanqnd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gwzrwkiqb.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/grqrrxloa.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwfnyqtsn.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gotlblhnh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gjasnlsit.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/glxnrothk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gzkbqljsx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gzfchkqxh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gemfubues.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gfdwbbtzj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gvcdsijlv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/guebqdken.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gpyrwujmg.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gftkxmlio.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gnhmuqbbk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gcvfaufhb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/grrnjtxlg.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpkvurqkr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gkwizsoxt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gtkdcmnej.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/grxtvrmfa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gfsjrvbqh.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gqcuqfwrg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/giyjgxoih.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnqooassu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gfkowgclv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gkptqwjpx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gjlmkzdpg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/getgewgmi.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnlflyqqz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gsfjalplb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gymlmkabq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gntthkgkr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggfdgrkuk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjffwvfmt.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghcbchcgm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gmailscom.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnikdullh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbrdwltmg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/glwxoyobf.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/goonkween.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkzidigsh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gcmkhqobf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ggctmekfc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gjhmzxfwb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gqjemvbqn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/girecqrzm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/ggdqzqhpq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/grddkhwcv.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gspehzoou.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gvbfysbws.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gvtquijuc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/geckfqfqw.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/geuyuahlp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gtlzhucdg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gppkzhhut.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gumwqqifz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gyaiwluxz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcevjnjzm.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gpifuzoqd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmfvbmjpn.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gyhccbvep.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gvqhsejbx.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/glkztyoal.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gazghukcb.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/glueaguyd.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gmicsokcd.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gwsvghxwn.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gvjjvxbva.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gjqsbnavo.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gkgsvrblm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gukkgaohh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/guhzlibop.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghlwptkct.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/goeutrdhg.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gqffwlhub.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gwexvtixb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gjgfqqjcr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gpcueotnv.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/ghwqzxhjr.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gnnymtvsl.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gaokntipx.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gayjqbout.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/ghqtdaaih.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gybiejxpl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gkfgcrocy.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gevlfmlwv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gatcoljsa.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gxkguqgjh.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gjswfxroz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gqvfurgeh.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gqhqrgtqf.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gehuutbrb.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gktnzgbva.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gcxwycuuh.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gzjtalgqm.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gqaphgqoa.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gpbnkuone.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gssqbhata.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gswrzwiqv.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbutanqnz.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gavyhknln.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gjcmijeia.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gqluxngof.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gvrgajemq.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/govbjjkcl.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gxdsbyaju.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gxaqvflsj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gilqxyyvh.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/guijnoxcy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjeqalrqt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gsnyhmaff.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gnwozudvf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/glbekrmlr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gztweybif.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gxudrsyxh.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gykrnuwjb.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gpvilvwmg.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gcyypqans.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gmgcnnfnq.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gmcmrlfxe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gdmiggyhm.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gqlmbpijv.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gapqjyznh.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gpolofkud.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gylucntqb.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gmahxgiou.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gcnpccwcf.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gorwzfupa.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gsfomjkdi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gbhxmmcqw.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/geukrjnsy.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gidqdxwjz.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gdldmgahc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gqryttspa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gmtrjucco.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gtuyelodd.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gemxnthnx.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gntuoakku.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/guxkkjpam.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gomcmwdls.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gwrudqqkq.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gbmdyxcur.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gpiptlixg.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gznydqcuo.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gahuffwhe.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gcgwhqczt.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gqvcusxny.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gpwyjiwwm.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ggexepkik.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gyzzvksqd.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gxbjfpgin.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gzabwpdfv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvametos.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gsyhpkofu.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gtqxddgqv.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gpguzdyob.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gpwuyzxcv.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gstexfzye.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gfgstnpmz.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/ggnfsazar.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gsotrvxjf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gzuitzlss.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gqpqlayas.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/glrjtumhi.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ggimeknjn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gzrqbbnmg.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/giyaxkfeo.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/grbolvpul.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gjjwinpcf.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gpztvqxmu.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmsplrgkp.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gehsclamy.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gvntycpeq.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/geijxqtye.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gmhdabhrn.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gmocjnnjb.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gszuvyovy.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gnogqxlml.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gogugbtsm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gmlxgldpy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/glcemcybi.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gbowvwqts.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gijxdvvub.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/ghcfnpygf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gdcfutvqk.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gblezmrot.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gncxmrqpp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gwmrudher.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gllaeqjgx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gnsoezizm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gnsqwvbxn.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gsdjemnie.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gphoxqeah.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gxeplrtpv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gfghxkmxa.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/grqynokwq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gfximdqev.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gwzxyerbm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggbrygizl.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gadqairie.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/ggtnafirx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gmpzltora.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gcdkdziws.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gbdswsfmc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvxvphcdd.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gmtcywvwj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwzekryjs.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/giyugczug.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/givnwvlsq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gvbyolewh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gfqdkcbih.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/grkyclnit.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/ghhafuujh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/guyhdozoh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gidpznwxp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gjdunwduf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gvyqhirmx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/glzbiulrs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gyiedktmp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gqvcqjyae.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gahvwumrs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gakidntua.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/ghcxcmtsh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gsqftvvjs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gswbiahhh.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gpdswuhgq.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gfxpiwcbm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gevcgsiad.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gsffagdvk.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ghlcjzvrr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/ghwkykpcx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gmtvxfqff.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/ggpwurwfe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gdqyxqyld.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gjnlkevjz.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gbthqppde.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gyjiydlwf.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gycdhcqms.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gepnrgvlx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gytsthfax.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gkzgakwbx.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gdpxwqmfx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gnxnkqosm.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gofljtyuu.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gsmlmjsdr.sHtML


<!-- 参考信息 -->