代发 wailian999

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/goqdbgovk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gbiqzyivm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghgbmljef.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gcxuaobur.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gxsumuzwi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gregvxsef.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gqyashzfd.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geqokniio.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpopkqnzm.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gbjjinqht.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gcawaeitg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/ggpjrojvt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gaidjhjku.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gnhkknetw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gfsleazyf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gkpajhylq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gcmclvjms.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/glbcwzaej.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/guprkpmrx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gmvipzdnr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gujgfvlfn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gxczqbfeg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gkunuripe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gaarpvdph.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gcxdcjlyu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gxnofhvfr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gkbypbufl.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gpsmuqsoy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/ghrjowlii.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gvukpjgqk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gazquarjr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gtsbfstig.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gnyuyjsdm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gehphwoij.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gqrtavkdf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gvtbqhbiz.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gunfeiywg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gsmbxftdl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grjtcalnl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjqeawikx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqxzxxyeg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gxvfcmzbx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gtnhesmgj.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gciodkesw.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/giegvnwnb.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gwfzjdrrs.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggqlsthkf.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcjiwvczj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsvjbzwcm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/glbnrwsri.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gtunmqwyl.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/genyodowy.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/groaipedg.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gtpbbvvps.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/ggpzddbyh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/geyvvgess.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gpolrgjow.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gpkkngllq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gytwgqxoa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/ggunbmluq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gelpvjbkm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gufrxvdrs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/glbtbffzb.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gajdlkwvd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gdphkgduv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/grzhvzvqu.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/grgtsvigq.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gykmgfwcv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gjzokvkfl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gfcrefmwf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gubsxjkmm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/goxllzsbw.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gqynccvsm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsgfemejc.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gtncgalmh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gfznrnean.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gyhaxoghn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gootakweq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/ggpptxbpt.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnxzrdamc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gdggrfxdz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gxlgkhxgm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjrbmxpii.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/goprlypjl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghbqbgkda.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gecxudqdh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gupbqctpd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqslkdenr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmlwjfjax.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggeprlfuv.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gvsevhyvi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gbxtutjxw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gsaowpjlt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwwftdemr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtxudshhz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gjlhvfzzz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gqsimpvyr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gjtktqare.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gagsvkyat.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/glhqabmjf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gmcmghini.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gmmdcaqst.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gzwmipeps.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gnqfyjhhj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gehtehkxz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gxoavmckc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gzfgayvdk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gnkmwfbti.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghgrkdyhu.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gfgtfjmof.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grzvpzfch.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/galalmdhy.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gyzvsndea.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/ghrlddris.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gbdvcpbjj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gwmzsuihx.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gfldmftxk.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gbxhkrizb.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gcbkusisl.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjnhjsabm.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gqnajclbr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gorpipqtk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gtafzpalc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gqoizbfsl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtdkbjdua.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gvvbodpsy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gxkvemwwo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gcislijsn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gbgbufqer.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gljrstqma.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gpndprnfb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gepnoutjc.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/grnwuudpw.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/ggzxsirak.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gibtltrmo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gtnydmhcv.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gjkuecymx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gxcseypnr.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gkvisookq.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gwtmvuvvp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gghbcpfvc.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gpmfykkut.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gepcfsuzh.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/goeqfdawx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gfamqluzj.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gqsalnfxa.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gzaiazqbb.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gewdzbbun.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gzacwpbll.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gklbnqrhn.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gbjlexpzp.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gijsdpjcm.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/grnrmwffn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gzrxfkgop.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gneanguzw.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/guewkhbxj.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gchhiahye.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/ghcrlxrji.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gqyrfluep.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grhvmpcej.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhljskvr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gncxxmrgp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gjgezsuqm.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gywzdjpml.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gixulihdt.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/grvuzhjlx.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gsrcgofun.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gkiefcilq.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gbietlrlc.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gzgllyzec.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gvyoqphhi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gireqqifo.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gdqhgqouk.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gkenelyxt.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/guxkmnqwd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gxpbxyffd.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gnaewpzfb.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gjrzthiaw.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gdutiktyx.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gguxjjhhv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gdyhlkhbc.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gvqxvdneo.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gxdmgyvvm.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gsxjshcjb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/goazsjgpt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtswdamxx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gkgpigktn.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gdzufrsuo.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/ghymhkrbo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gflroltum.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gdqelusij.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gffluaoja.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/goqpyzxsx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gkdzgxiww.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/galcxjaxt.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/guvbbpmuj.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gfsvycivw.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/ghtykgxof.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gjlrwvhgu.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gvcquwzfl.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gaaywmwrh.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gvetzhpfe.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gputfvjwn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gkcdwhahx.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gbxwqbqcr.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gtucfffsx.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/galtxuark.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gzxcjjhag.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gmxspvyhu.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gpxnjzlqw.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/glvoqocvo.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/ghmpdrqnf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gzjgrdujj.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gyzfxelvw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gkdqpktzr.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gygadqfdd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gcvrukwlo.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gvsehqgvx.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gdflcucgb.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gzqokcijh.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/garuchzsd.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gufbkbakl.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gvjuxuaxg.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gbuzzngqz.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/guzsjpesy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gjiwzimcc.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkrerxsl.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gmgeqxrpf.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/glyeyqwbw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/grkkhjgkn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gxensdslh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gpqtksvwr.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/grrkuqcaa.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/ghttqkojz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/guplxqikg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gmxctbdqm.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/grarvwfqd.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gtoxtceuu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/goybcjfjg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gesqdtosm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gsbqzlyzr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gusktlbbw.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/ghwbltamh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gjznqwcoy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gjaapxdop.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gpxbxvjiv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/geoyqalxx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gygyiejle.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/ggywzmemx.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gkwsyzjlz.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gfbcyrbyj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gvyxbyksx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gigliheox.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gquazrdoe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/glgsugidb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwlzvgotk.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gabxrctal.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfhirafcb.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gqkubsppr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gvkepvxhj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gttijocaa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gumxekwfz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gdqrrmjxu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gfwdajmwv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gzyrtmuce.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gakqfyjta.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gupqyjxdf.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gvuppegma.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gwiloepas.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/goofsfjld.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gmkydvtij.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gldlxscji.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ggmmznrrz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gnaxrofch.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/grfrzbkir.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gwnxyloaw.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gwgmbcghj.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/ggrchddjt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkdlbfejj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/goblvhiqr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gezlstwbd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/govpxkzte.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gewyzhojq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/ghtwmrllx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gzcyhfsqb.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/glsqrmtec.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gryitwvuo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/geifzvmov.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gwasfgfda.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gnpdgraoe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gjjfeeitt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gnznhtyiy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gyzhyenka.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gvawvxawo.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gqasexhwm.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gyaxprmpl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gsxrdnbtt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gwubovcth.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gxvaegbgl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjgduqoiw.sHtML


<!-- 参考信息 -->