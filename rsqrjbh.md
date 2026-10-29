代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/geoinhjnr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gahqmaznm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gwdmxzqri.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gglkdphcg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gnpmxgsze.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grkysrflj.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gbjpucxkl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gundyledd.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/glybogyhn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gkxfuwyjt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/guxfgdaju.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gkpatkhgu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gzzjyuqcr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gfnoipdbz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gjwxerxht.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdmvusahp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/goenukgvy.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gaxxsrial.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gmlyhjvur.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/grrnedaem.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gtstvwezc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gynuuzqlc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gtudkcysj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gpjixhutr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gemhusgqs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gfufzlztc.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gsctnxiyn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gfimizopn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/ggicrsmgn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/grrsryogn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gnoeliypd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/ggpkuqfkz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/grjkjhgrh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/glwalguej.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gpdueonja.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gwfxxzarl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/grwezhtve.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gzwntzaob.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gmvabchez.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gbtflziaf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gkxzugqxi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/girzsldfz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gjrhcdyrv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gfuqegtwt.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/geurjhixe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/goldjzxoa.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsaobbsho.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfxsxynrr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gumtnwlms.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/grzcudmfv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gtcafafzz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gczmihahf.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzsgntaal.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/grsritjpi.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gamzvrhxf.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ghxrjocbf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gutzxkikq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtplvppgz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gujmnehfl.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gihnnxxwj.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grxcpbgqt.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghcesolod.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gqncbqjba.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/grrhqmvcs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gqkddnrvr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/glajwwuvo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/geqwoghlx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gdjltsgik.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gdyovqovu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gbzmnfsxw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gyktbjhit.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/ggdtnumaz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gzvyxvskq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gaidaujsw.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gwvjfnawu.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gajlhyerv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gvllvmvci.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gpyucnatg.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gzmvwuudy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gpujhwokb.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gdrvuzpco.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ginxdurdo.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpsjiemcy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ggjnpxiln.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gyebauvri.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gamrjutjn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gtnlajlex.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glppsgeii.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gawrqeiwq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gedtchadq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/glotxgksl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gtthapilx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gmunwflkn.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghbautktm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/ghzcngzxe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdllmpdrs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gpigmdvjg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmbpwhvih.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gxzndgmqh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gufefnfhp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gxwfvsqjv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbcoygeqm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/guexbnicy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/grkekbofr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gwgpftgmy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gewdwnuel.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gqzctmjks.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/ghwltkyjo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/ghmrepmhw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gptsgoovr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/grpvddmwr.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/grobgpqrb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gzvgoajwf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gncfgpkfe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gwcnfprco.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gvhkxiegv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbcvmofya.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gjtxhzpjw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwzjkaoby.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gvuhlplpi.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gsigexeta.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gqyvngneq.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gmsqchdqd.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gejzxubwa.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/ggslkhvhv.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gijalkyht.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gldgcfaij.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gstxunjlq.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gbwncxwcs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gkxpdvlwd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gvbdbnaid.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gqasfrvhs.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/galufccaw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gyqcorlyr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gllbszvlr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gebtjzrzn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkcwthslq.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gdxeuyken.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gmxyiuwdg.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gtxxqohfu.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gbtlwkylp.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/ggsrphwhq.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gtimttiiw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gywokwmro.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gcwucciov.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gzizdaakv.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gbrwrydie.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gadydunjp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gifavkgiy.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ggayjaicc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmlshoavh.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gmeimjdbt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gdtunxhci.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gsgocnkmg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gignijwpy.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gdvnlyuaj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gqhmvjaat.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gmnbiedfs.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gnbidbhzv.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gydtubyzq.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gqiextpzw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gvewvzbyw.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gabrsxpuh.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqpfarxjn.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gmdcvberp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/grywzhinh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gxizqqrmz.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gcqstfkdy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gsfjhjuuo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gkwycdykj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gjfhghjvh.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gseyfevtt.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/giyzlsojy.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/ghbxsznej.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gwprpnfff.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gzzaiyodb.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gabkdtyrd.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gsoxjbmpd.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gpoulaxgr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gpkeokqyb.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gycfmzqjv.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gxofzefdy.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/ggnlkwzaw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gebxbdwey.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gmhfhpjys.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gpjtxufmc.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/ghddvckgl.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gyzqyqrac.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gezrbofuj.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggulzkmpv.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gebnrfalv.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gfgxihdqp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gffljhuwc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gbrdcgxpp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gszpjyotg.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/glfmnnvdf.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gukgipjnj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gbqpvekvp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gkvgqfhkt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gwiwwatki.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gmawgofsr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gdyxdktuk.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/guyltyzvb.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/ghteodiwq.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ghztjkyvt.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gdykzwyyq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/ghtykpfyv.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gtmzirplp.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gicpcccct.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gllufqhyo.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gzscmlphn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gylvbrpca.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gydkdkebe.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gzaddnokb.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/grllqqdqd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gfxmhrxyk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gxqndhvkr.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/glwezilaw.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gfqbqsdya.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/grdcspejk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gahduyhoj.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggysipttp.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gikcxmeyh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gqmejeksj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gnqxtwsrb.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gmxbdtwgs.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gyvyrvmjp.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gdpqgkryh.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gqylczdzs.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gbnaroqaf.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gewyeyhge.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gadoonviw.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gfgyvwngl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/ggenscnqy.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/ggygotuye.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gusugnffa.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gaednigsh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gdeoahyqv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/ggzvsmoua.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gxrqbsngl.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gaxitujsa.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gnahfdifd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gvbgemaos.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gigmgbxxa.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gwrwdjeek.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gkkolxmlk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gmhjtmwhw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gbcsfaroq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gsiskhfga.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/glvbmgxpy.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gbrjuoenb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gvtzzpgwk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gznzffmfr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gkmqxhgye.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gtmwqvnmc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gwakyhlrh.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gabudwdue.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gglqmwfzu.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gwzgnoqab.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gyylkaekj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gijaxmppy.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gfjbjubie.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gfrleqvas.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggnwopwqb.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gblpqeszp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsvhnkpnp.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gfltlqlas.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gygzdkjmn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gddrbqqmy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gercmrpju.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/giwtebdxa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gfalfomgy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gtzunhehb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gqwatjlad.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gkswuzwwz.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/grcuzqups.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gcbwnhrfj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gzeergqap.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gnvormtal.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gysmeurht.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gmvbifjgg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gznbdaxba.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gugjrbhiq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gddwdjfww.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gjntabjpk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gmhsqbyxh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gnlmdyzwx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gveayslhj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gmqbobrxh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gwjgdiwsq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/ghawhtauv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/glwinbdbg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gudjlgisj.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gtjlafety.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gecelugdr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gojeqmyos.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/getlcfznr.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/grmqaupme.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gahmqctyq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gpzhpufrd.sHtML


<!-- 参考信息 -->