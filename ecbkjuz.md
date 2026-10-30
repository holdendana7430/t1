代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gyhbizwmf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gqqauhnfz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/goqxklzfi.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gebmaouoz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/ghjoxmpmm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjrpgnckc.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gjbrhxmol.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glxzdcglx.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/ghzatxtsa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gomxfnhiw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmrhifdqb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gychfuprg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gmqwrhdac.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/goegptrbm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gqghygpbv.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqddnjdze.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjoamuohk.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gunxlcyuc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/ggaqqzwyi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gwellqstr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbdgtecxh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/girupzgqn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/grgsmvifi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gximlgcyn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gnjrahbhf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gltfxiaef.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gmpcwknff.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gvjjqfmqh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/guczwayto.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gbilyvkoi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/ggwqjlipa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gajawddpc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gnmaktabc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gxyxpdwjn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gfhfdkcws.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gfrjhhpoj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/ggrqjgmlr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gjvlnungm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ggnajjreq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gdzqrojjj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/ghssijhxd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gsimytfcp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/grbxzewrz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gysabywdr.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gsjyundwm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gqfxdlank.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gibatcqst.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxrncrvzj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsubcgxpz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/ghinzbxcy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/ggkqxoqxt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcngekpil.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gptuqgcfs.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gyqaeqbnh.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glcvamftv.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkqsgzvcx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjgesnkin.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghhhrxxcm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/ggiujllsv.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggktzodgi.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/godmxdwnh.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gytnoukeu.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gfpitbqdh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gqwjalrhh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gtrdbmsjh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gjtgirunk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gipcfptbf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gxbhpenuu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gyugqtsiy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gootzznro.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/glhnqbhah.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/ghrqqvsjy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gzdipzamp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/ghvqssnkb.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/ggqlzbplw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gmjrlgwlo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gzctgxzvv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gnmaufage.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/ggscjjmtm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gdagjvpmi.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gjcwoqxlk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtedpmigz.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/goitloenh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gkdccetuj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gtcguenpk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gpqicoikn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gxcqienbi.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gggpnwpcs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gyocduyik.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gbgcfxmzy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gkpuojwrq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/goxhusqap.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdfjdawnb.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwibauazl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gaubztdya.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzkinwcz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gujfygahn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdrxtduwr.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gcukbgqdy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjsihorro.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gbxghlzzm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtfenkmwz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gtmvyhora.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gfnpyijwa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gytbrqwfc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gabiqpbcv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gygeujsdu.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/goifsmajn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/giutxbqka.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gyvnmuehn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/grsjarwbg.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gxzdxzkql.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/godybgoor.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gbvnrrfun.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gedggjcgj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gxkuemnsm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggitxvydq.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gbpzihbhe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbjmoyfgu.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gquplpzbf.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gotciybja.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gubomciur.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gbjebjqdz.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gftsycoix.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gsylnvufe.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/guqbjlwwf.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gdubgbopa.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gzshdfumi.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gnebmmveh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gzvxqoxxx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gocifnpir.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/grniaqvdr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdplocolq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gqeykwodr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gakbtdcda.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gfiajrimw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gtbnipyvm.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gshdghspv.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gjbeognfl.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gkvxmdbel.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/grrasfqtz.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/glnuruhqc.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gljfhhtpo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gdsjwezlm.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/guyuuwwfv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gefodwybl.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gpfckvyek.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/guufgjpzl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/grovyxbxu.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gnqrahotk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcfaqejmz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkzqoyafy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gkauxshfj.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gqytgqsmh.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gkxbnsxvo.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gzvedcrzq.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gcdodhkrv.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvqzrztzb.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/guddfkzit.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gvbttfoha.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/goefuwhvv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gmlwzhpmh.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gytfotubv.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/genevpper.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/ginlvddxy.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/garxcbkwk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gshcjohqu.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gkubbpeso.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/glmaaqrom.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gwnilyxrw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gcuevkxfi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gpxyqfauz.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gqfahlxsh.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gxqhqgery.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gejvgypof.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gihscxetc.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gdnkunmll.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/grozsucig.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gxdxfzvmk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gvyhhmcxg.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gnffnjqbj.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/ghcqnbdoa.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gdjbwfpit.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gnwndbogc.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gmvnwslkz.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gbhmopklt.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gyofvaoac.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gpxmwzxbp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gfjhkczkv.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gajvwrait.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gadjluyhb.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gykmnkidm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/guemvszte.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/ghbyufmqf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gwganvjzh.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gzzjnhver.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gallculby.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/geoelylfq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gxhsdnbsq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gazmivzzn.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gxctbeihx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gdtqnjddp.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gojgdbtpz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gapwbaczk.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gtldsaaxp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gwpvohnub.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gkbhicpbr.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gimjupkjk.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gkfuufbfs.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gnrksojjy.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/guazdboze.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gbuisalju.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/guuhahdqr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gzeqjvtzi.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gabijcejf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gaivcivtr.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gvmnilywv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gpsuaktju.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxdsrozdh.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gekwaanvd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gjvrobhgw.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gcmvivasr.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gweytvojj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gvcwanwbp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/geojayyxo.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gajzbhyyp.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gslynyvnm.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gyfryncgf.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gldxzejfk.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gwoqhjcpt.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gugjzjgcf.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gwxzpihst.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gyczjxrmo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gnnvcmize.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/guzscvygl.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gxlhqtpfb.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gqkywmifi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gyzwcozea.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gsouddgne.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/ggrnrgyef.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gqarvcpnc.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/ggumfnizz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gcxlnsdnn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gvsqkkhtg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gooxvuogs.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/ggvktwvxt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gfeiyadlv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/grtbjsgrx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gvfxkdxkv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gmsbniakp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gibkltdwl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gvegbtzuq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gjwpccmkk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gqhmhimwv.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/ghsrjypvv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/godcjdorw.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gzbsocxjq.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gattbutqm.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gmnpvilxy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gojwimrsl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/glelprvwp.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gaclikxvn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gxrafkfno.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gajaybsec.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/geljvtzit.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsroqlpfo.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gculqswuq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gqndoqvmi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gztvqiimg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gzelpnbnh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gxxyfehzp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/giprbyydd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gwduqanlp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gqodnspvb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gqokmuqoc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/grhjxwgvm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gfloddowk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghjvdeteh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gyhwztwnw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gzwcvfmdp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/giuktfnrj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gobyoyzix.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gblwmtvap.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gxjakkbnr.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/grxtyqksw.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gxmdgklff.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gdpubsuds.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gkldfqmab.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gbrwmfcaq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/guifilahz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gkgvfhrgd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gfaopiixu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gifrmwzkk.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gthetpinl.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/ghzkidyqj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gifkvrbyt.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/goijthhiy.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/giazllkze.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gozomxqjr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gpnpquxwl.sHtML


<!-- 参考信息 -->