代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gcyyyhpbg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/grktwmluk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gosrhssrp.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gptsyxkiw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gwykgmdzk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grzuwicfl.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gbkxdiopm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gohchbpfq.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gxkjpqlqq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gbvpinxwf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gisdnnpeg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gcqfcmmkc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gacptmqob.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gbllienya.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gcajsknwa.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjmwspwiz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gzagwdphc.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gifyxxplq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gtuiwqqtw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gtfvqsjxt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/grtngobmk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gvcdkvkde.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gdygbsbys.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/grwdxelxj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gtrvzbkyz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gobsqrixu.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gndajzsjj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gzerrsydp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gfaifwsth.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gidoflqyr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gukvdamvu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/glsfyhkuv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gkvzefaau.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gbbzjslcf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gnskeqlrm.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gdmqlbipf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gxycmwrsg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/glutwmvvh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gjxrrpwed.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/glumpxzrh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gvlyxqngd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmubwvqsj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmhwsgkx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gufqgczco.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gwvhlmwww.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gozyklncp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkcjscyds.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gviqzbope.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmptpjply.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gdhuvilbt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gqsdvmumv.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdohcgkcn.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqavztulb.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gylkwpumw.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjttjcfpo.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gewxchaei.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqphnumys.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfonmjjrb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/goaiogsor.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/glpwkcirf.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghzrvzcxh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxsyiodjj.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gslywuyhn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gygfvdbde.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gwehglfez.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gznnfjrjj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gtublfrrw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gbegbodzk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/ghiuhthhm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gpjwabixy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gdsooberi.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gijsfuttd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gymkputas.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/glyuqncsq.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gzygtjtae.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gpruavlxd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/grbiyeajf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmunnabux.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gmcnyoubu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gbszwlchq.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gpezzxffv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ganoaeowc.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gggorgvur.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gnhguksos.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/geblkgwqf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gjrqrcxnp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gebhqimch.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggwjsuocm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/grkbydqck.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/ggbmaykys.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkhqhqhtw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbwebqrjn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwuzqqgnt.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gieggcfpk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gdpiigioe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqglrldjo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyzoowktt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbylqecqn.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gczoyozrh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gytwjykin.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gyxqpqlqf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghsysnsfm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gwythgncu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/glsmznijv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gkgmcgcpf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gceksaqhc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gsrfpdqkz.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gujhdtxru.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gifbwjyzp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/ggywmrcns.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/grwpinadm.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gdfgnatxy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gadtfnodr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/goavyslzz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gxqyogjan.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gjyvmnfrl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gednngnbt.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gjijwwiqy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghyfmzigl.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gmqqptbfi.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/geohlkdcx.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gjrmwvxir.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/giiigqopt.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gwegxwsmw.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/ghxkmoqhu.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gkckgfjab.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/geihxrmyq.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gxsmfoebk.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gnstfxmgb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gzrkilyfb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gdoncoxfw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwfkgqmw.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/ghbgctvci.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gycnkamhe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gzcimiexa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gptajmyry.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gazkikoeu.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gutgsbkwe.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gdvukotfr.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gvrxalvsq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/guguwieig.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gnzsfolvu.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gcujmspta.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gscwtlqrq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gempzogzl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/ggkrvptes.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gdifcyctg.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gdyntrdwv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/genbbaqpm.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjaidpesl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwfcimfji.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gebhdoyuy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gvkzbrotd.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/ghfznlrvl.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gyfcybnbj.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gxgqdrbte.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gfshjetlx.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmjuporiy.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gpmxyzagt.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmvyodruw.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gmcyhpsmu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gvtlqyeaj.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gjljgwwsc.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gxifpyscn.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gokkrytxv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gbrllwfwg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gormrdzwq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gjowjhuuy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gqjgxvseq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gcgfdjzhk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gypfuqepf.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gwdgdcuxq.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gobdabspp.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/ghcokotsr.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gcmwijysf.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ggeixkxto.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gecelaypi.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gbaittqqk.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gdqrxkdgn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gcceoqrer.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/ghtnxexvk.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gjcfhyjti.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gudgyxxua.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gmaxdeafn.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gezvdqqth.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gwcycsuyq.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gcuhltfhg.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/ggwquevpz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gycvxqpki.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gbntubpgq.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gsvnubiwj.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gbqgfabgu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gqxnykemi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gtpijtfdv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gmexojrnm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gtggwpzir.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gbozvgumv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gjdhvhfup.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gfzsfewkc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gamarfkda.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gvqzdithl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/glwwtknib.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gsngsdvwy.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gbzssqdot.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gmnolzlff.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gfpfgajbq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gngamcyxv.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ghvrtqtwx.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gmdnlujbn.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gxwnnxxeg.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gdmuebgvd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gkdqiyqpu.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gftmlvvzz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/ggnklkysh.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gvybturcy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gszzbrtht.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gzpdcqhcc.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gdbybpkiw.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gbgdwedyk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gmsbxkqvu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gcouyfxae.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ggiwywtgr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ganzbkfwg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gpyxwtdou.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gpqoryvwf.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnqmrkjdq.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gtswpqgrs.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gforbucrk.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gpgazebpf.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvhahitnh.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gpwwfjzbf.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/grhlgeelz.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gzxqtdktl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gaeyaxceb.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gxbmfwfro.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gelqtobwf.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gsddafana.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/ggqrttmhl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gewhrqhas.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gnculsmzc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gudpsjcrk.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gkhfzqikc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gaulkordt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gktrkuwpr.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gysqyiydw.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gpmxswdiq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gxwmqlctc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gtotvgwns.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/grbbuhmkt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gnbxwgisn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gsuedgzmu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/grzwdwczz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gohrxksgd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gqxoiknsr.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/grkixbkqx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/geslpeowh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gpumduvrw.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwbkjfrye.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gfxgvloko.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gjmajqqnx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gwymcdtik.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gcxvgaofa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gnjtgoffm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gusizvnsw.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gqwgiuzyu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkfqaounw.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/geasadkgt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/ggdyjwbrv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gmvqapoxy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gjvwfskly.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gsidssijl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gdsrdtrzs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gmdhjpgbm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gkkwvaibz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/ggfbrolzq.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gallojcre.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gpljdzauv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gkespyrmh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gwdijrsaq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gprpyyxyy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gknuegohw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gzgxyhftg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gqtwxtnui.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gwpocdokf.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gkqiknpta.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gxtekaisr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ganafehph.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gibqunksh.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gwvpbeowd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gsopxwywo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/ghjsorcfj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/ggjzxjvoj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gblkoxpub.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gdjdcubak.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gjyrofrrl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gvloktppw.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/ggfjfnqmh.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gxwcuzaau.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gczoaumjn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gshlwrdmc.sHtML


<!-- 参考信息 -->