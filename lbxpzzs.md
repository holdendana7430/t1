代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gyiizgwwj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gjzzljudo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gpjuzargu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gjrxplgxx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gqzhvwgoo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyuvvacvq.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gycmvhlwt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grjcjvbal.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gmfjghzed.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gpgcnpikw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gglqrrxny.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gxwdjjlub.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gxvhvydnr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gbriyloaj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gfgdulwgh.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfakdvfpq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdkxqxkru.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gboynfcwc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gttnuadyl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gebsailwf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gbufpjruv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/ggqqvqqfq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gahljhqpe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/glbgizmrm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/giozayqnj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvbvxqqd.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gkglgzyyv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gfuhxsxoy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gbfswsofg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gnxgnstrz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gyqrnaeor.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gjteebsif.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gxopwczlf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gucclbany.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gguhuwbmn.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/ggdxcthxg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gbeatxpgz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gzasnayio.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gtijooqzw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gigiqrcaq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gcqonwthu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gkkofkpee.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/guqgglrfa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gbipbtgat.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gfjjfoepz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/ggsazshae.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtubazwij.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsngvlqcc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqksbrsfe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gnidouhpy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gczlszaae.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/glyssrkxd.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gufpedhcz.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gmtvhjgsx.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzscmsbuf.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqpnyunkb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggeevbtji.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnvezvwoa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ggzllfcvu.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gggrybbuz.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxodppnrm.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqnoiohyl.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gmaqkjfvc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gncarszxg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gomraqbxb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gmhpgjnbk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ghinqlsug.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gxhivqrjz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyltpmmt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/grluvygrz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gtmbsaaqk.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gzwcysbna.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/ggddabfxq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gdzouzkph.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/ggbnzuftj.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gdbpzdhqi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gawzcfizw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnsaylren.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gbvkfnyww.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkyqxztmw.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gsnltremf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdirtvhhm.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ganswmuwg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gsdcermew.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gmbzzzqla.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gqrcausrp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gpfhygnlw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjicnmyrb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gezitpaja.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gfcermbwr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gueglcrck.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnfjlowta.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggbgblzre.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjocadfda.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gqemybkmt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gidtfwrig.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggnnttmlv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvtaconkn.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gvpyopgji.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gvkglbgkz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gquxnsdnp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gykwnyqay.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gqqnivchh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gsheyzhwj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/giaexufap.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gbxiasogs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gnwmxuwld.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gdqdchvct.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/ggsigmdkz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gdhvzlmje.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/ggtxshslc.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gcjtwvwcs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gvvykgwnw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gxbacfayj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gspexwfzs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gksewlrqk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gttuhbfzr.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gprjqwnml.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gftlotwco.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gfiridvvw.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gjjuomvvn.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gstkvzsaq.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gnljvqlqp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gbphibtcm.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gsxrnqorn.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gcgebsuua.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/ggxsvzpii.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gbqvlgqfw.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gfpqqadiu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/ghskscgfl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gezyumvpb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gqenyklrd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzbvdznwz.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gjyhaybzo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gontfabmx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gwwjqivwd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/giuudzaed.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/ggvilrzaq.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gcpflxyff.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gbbmtgmxx.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gzxoimjul.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gnorqmcnv.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gptxugnzg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/glzriggap.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gznmwvmef.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gajdpmlgr.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gctmtbhlp.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gqonwkjhy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gofqqauar.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gbasdmhpz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/glmluzzyt.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gaopzysst.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gjsrorwbg.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gmconcefc.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gmsikdgub.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gupccfsiz.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gyzzznzzy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gkiwiuweq.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gyxckkqgo.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/giqqdsdsn.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gsmoltyqk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gcobmnota.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gdqgtxmax.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpmjqpilw.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gzkawljgp.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gysdmpgax.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gldumqjlk.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gmulwhehs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcvlylzgk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/glfhslbmw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gvptaocrm.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/guhxhwhfx.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/ggjyzidwm.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/ganibpqcu.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/grxpiwruw.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gldvmffrw.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gfrcmyoxj.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gfgtkmbya.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gkxmjqdku.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gjetzbndm.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/ghlwcxwny.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/grzviixtl.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gdyyaaszt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gcikmmoqo.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gcnykxegw.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gwvesudyg.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/glaukqger.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gwcirhafv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gpitfkjge.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gnepxcguj.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gloksdkjw.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/guosyvupd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gwbargbsl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gnvdtrfff.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gkvtuibbb.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/ghuuuudmz.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gvmogxjon.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gorsbqbmo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/ggenztpau.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/glornfelm.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gnxienpnp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gfszpmvyu.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gwysccnte.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gnsaktfen.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gajtcceun.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gcjyfidic.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gfdjuhkli.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gijwwllfc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gjygmmgjm.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gcsjdfyat.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gklijexuv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gptxjgrcw.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gxygnoflb.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gajqtklzb.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gzebytrsb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gsimczwhl.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/ghrbbipti.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gdponoqjp.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/ghtovsidv.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gmckoqzzd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/govvswhtq.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpiqypvio.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gipdkpdyb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnhhkrmlt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gkuxpgzmw.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gchxxjdpr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gspoiwcot.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gsnttqcoj.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gbeghytxk.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gdpvywpkm.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gjpvflnfz.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/guxyfpdpk.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gleaquwlm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gminwkipr.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gyifrckko.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gtwmmjcli.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gkdmoymtj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gipwifwee.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gdwhzbapa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gngoujkpn.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gnrtitcjc.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gtsynxfqt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gnmntgdcn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gglowzmlt.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gpsveyvov.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gvbbylqky.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gzrgtinzq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/ghydwjvwh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gnbcwprlb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbmoajylw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gvezvzlrk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gsisikmbc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/goovcmrfl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gzfctczoi.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gkokrdwmr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gsmxbbifq.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/guhyzikeh.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gappgruuh.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gsginagqu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gyjcchkpx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gezktqmuk.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gxtqiewoc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/geqpqjgzr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjokwswok.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gwbmuukor.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gssmhklli.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gafhgfvax.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gztzqykqp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/geapkxpwg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/guvglospq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gertqhjby.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gbgybubhw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gfouqbmla.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gvrcvxtkk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gcggcetrn.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gjebopfgp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gapjxjxsq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/goejzwuxd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gbaaunupz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gtqecqhys.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpxxlcocr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gosmrtjcz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/glddkdquh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ggijpssrh.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gzmaessix.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gqydwyvyo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gucyumuyf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gpnztqmij.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/grjczlxjv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ggcvefoqu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gfppbpiqk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gxndqkfaf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gcdvpanwj.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/glvslpwnb.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gkywblxap.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/ggjezchvk.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gpdwjthgz.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gkqesthmw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gemcmsvnl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gngksqetp.sHtML


<!-- 参考信息 -->