代发 wailian999

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gzagcjpzt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gcbuovdrz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gmqnqavug.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gdymxnnpc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gvwygmylh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gmhzqidcn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/glvcyhwlt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gqurtacmk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/groidavdq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkbzaztmc.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gtbpjdelv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnywynxgl.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gnuvtyyif.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gmrygmgqk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gliygaysi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gpmutrdfo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gsbmtnxgy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/govyoadaf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gfuxvuoip.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvnawjipc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxvkozysv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/giwdrwbqy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gjftcsivb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/grbzxlkuc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gzuuqoekl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gqcdmhyen.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gfnlyoomn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gxvdzsasp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/grdxcfbet.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gnnwxlgof.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gdrauwojn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gnucmxysw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gkelvepzp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gblkxhzqk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gmhtsjgdp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/giuiifysi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/ggqpydris.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/ggbgfkhan.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/glvagngpt.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gbczevadx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gteasftve.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/guiwjszuf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gdbpxeebr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gpdvpcbzz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/genvfvgfh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/ggbdmxuth.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/ggggfeceh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gtvjwklwg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gdiuvmcjl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gcpxhjolz.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glzflbkkm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gytzaphtt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghcuwgvia.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ghghxgptd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/ghquyvrql.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjcfevyfg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gulwqgnnx.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gomhabqdy.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqyxsydxk.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gesonmojh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmuynlfyx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyludqgwp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gdkjbkspc.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzormelmr.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giavcajbk.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gvzrextto.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gbpkbxzot.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/glshfqzvo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/ghlgifkiv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gadrwtidk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gpuyyzrpg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gxusayvzd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/glnneplzb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gdfsawmbg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gcareeyxi.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gffoayahf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtffzkbi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gpbzcfmmp.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/goqvptoel.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gsavxvtqb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gnehkjdjy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gxtqxqndq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gwlwslqsq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/guvxjvfep.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gedxafjul.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gypmtosro.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gmvwakayu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gtkboefdv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gkgiyripq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gpvctamyh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gbnqblyjl.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gubdjycnm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gvaajjhrt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gjpvcnhlx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtmoupbfq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbiujmwce.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxsscnamh.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpefipmpq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/glfypqndf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghwoyshto.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkdmqkgst.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwgxaxaej.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gkjatvjqe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdnaaapas.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gsvowkuhj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gfihxrwmt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gijlkwrgz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/goqneereq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gkuvybjiy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfotvvykm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gokguijkw.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/ggtqeqxug.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gemuukxpf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gmnrtkikw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/glvrtdcyq.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gqzyjmoux.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gbaamhbsq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gtpdywuij.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gtzznksai.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gnpbwesqg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/golyhahkj.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gfxmtfuxv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grgsykaim.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gsmamkmfh.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gdvevzoty.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnkjfwzlw.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gvugooltz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gksnkdaqw.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gpjgvzwzk.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gpacakgvd.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/ghfvmxxmo.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gonfrvsiz.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gvonnvuus.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gdyykgzhr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gpqvokryg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gpbknuxom.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gnvdneirr.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/glmuhoutt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gvewuelfq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gkgamqthl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gzvxlxogk.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gfprjuqdr.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gzulfkrdx.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gizpwkxte.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gelcqifzr.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/ghtcpitum.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/glxklxanx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gudijdvll.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gxlzhenet.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gpntkasyt.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gmsxomnld.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gxgpvgkiv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gocsswhjc.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gsjcpuzqa.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gaqbfctql.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gmfmfkfvs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gbpzmului.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gjgiioynd.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gkueunxlz.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gshmgkkye.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gdbhfcfwp.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gsivftcqe.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gjseithqf.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gzhqizrea.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjdxlzgzr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gxayrhlpt.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gpjjzyfje.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gzrzqxrao.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/ggxxzoljl.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gnlwhrlbj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gqnzupego.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gpgyzxnqm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gbgoefrkt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gplengqfq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gfeaiypni.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gitlvqfjy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gihhsimaj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gmxiegbfr.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gwhjwdvwl.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gescponxy.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gbngakzvm.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gfkemnrpi.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/grfblmqjo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gpvetvnyu.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/griarulyr.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gsbqtzfyl.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gkqmkszpx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gboptsrkh.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gndvgkcwd.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/glfitfjds.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gmgcmoutn.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gzhdrknaf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gybltrylq.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gzniqruxg.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/ghynosomi.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gyjepvsex.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gkeuhebmm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gdmcwddvn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gaqmvxnyr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/grqwudplm.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/ghraaolhy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gxtqfgtps.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gcgzuequg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gqdqcyiwm.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gzdryhkug.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gccklgroy.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gqbqoaavc.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gnrjmsuxc.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gkmgxyued.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gqhwzfrfv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gjhqmrpyw.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gehrfzqck.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gikboqpgx.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gcsjichby.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/glmhrmzvz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdlcosgqo.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gtwtabecp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gficlldtl.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gdppbcjjr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gajcrixgk.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/ghnphcrmc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gcggyqbhj.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/ghswuosrm.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gmxksyavc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gfuxxntwi.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gctzkbwly.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gzshdwdpm.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/grhhtkukd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/ghmhcbtoa.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gtxsojxlw.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gwkgcyxcf.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gapcvulhq.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gcfryntdo.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gaxgvvdvg.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/getkzoqpr.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gatbsswby.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/glqirgaem.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gugzwbpfb.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gjdledmzo.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gmwjjzhlp.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/geqwgdzir.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/geomtexyo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gdlhamsou.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gfqyzjvce.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/ghtjcfcwh.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/ghwwfayxv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gatwyhekx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gfkqcyxbl.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gaacjhqso.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gbtuwdxru.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gwrxxjqog.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqlzhmnsp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gbptzmfnl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/ghiquzmlg.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/grcfdajya.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gasgcklwc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gzfhtraip.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gzzgeoigb.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gndjhugod.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gvsxdhkpw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gyeyqagya.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/grpekzcrz.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gucaapemu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gmtisgaww.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gesdplgho.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gkxngbmqh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gmhnpituv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggxtwgjiq.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gwikkgrxl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkkncprpm.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/ghejyzytf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/givmagnxg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkasstwlk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/ggtjbmsjr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gelkgjfbq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gezfnlvau.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gbxgvavtw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gzddlfzhm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gtowgszty.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/grpfgmzcq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gjtnxprzx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gjoaalftp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggnsmudxt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/ggubfrves.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gisirquot.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/grouxlnmd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gglurhnbb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gbajavtce.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gpoepxdjo.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/glvlghaiv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gxzrsfzkr.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gyrqndqza.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gwnfcjpzt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gvwqwxpmo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gvfeyjjwh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gnspxmrwq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/glotccven.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gdriogwbe.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gvyieplan.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gfghrbdja.sHtML


<!-- 参考信息 -->