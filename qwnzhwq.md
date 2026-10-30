代发 wailian999

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gnbfrdojt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gydcxnnpp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gydnmafwu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gnpntrdwi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/glhegokdp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gpkpfrmpy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gsyjmuxrj.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gppubaeay.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/ggiilfhim.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glicposdr.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gofldblio.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkjyamara.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gydpldlys.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gdpdvljrj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzrplhznw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gtmfkkirv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gkodvcmfq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gyshwpovx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gnvivdmfp.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyxuvysmw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gkwpdesnm.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gpwgsqtej.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gejzgypor.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gfmfcvuzn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gxddgcutf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gkspeioxj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/ghinzfpcd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/grjuifeps.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/goqqulkyc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/guwdhpkwj.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gajkhagna.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gcozwfamg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/ghrwffihz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gjmgetuzp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gopielhel.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gvhwbvowf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gbrqkfsbp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gpzwrcgwe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gxikibhgv.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gboydyznb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gkcjacksu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gsjilghma.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ghrswwevb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxrwzmqyw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gtmyhavaf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gdaywkqmg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gbfpfbwys.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gahzgzlkx.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/ggghcqswh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gjvecmasp.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwxevkxyj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggfedhhxe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsjcpgnyr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gcpgfpjnx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gvdvjgfme.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtdlarpap.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzjkamcru.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gzeaowewn.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzywvjwob.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gslpxgkzn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giawqzmqh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gziszldol.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/guzmkworn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdtfhohza.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gflfkdktn.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gywwxtypq.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gtxfvggro.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/glurwtkyt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gngbvxtwm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gjnnqvdyr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gcksmmwvy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gikhkrxxt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gscgwysgr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/ghqqfjeje.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gtrgzknjx.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gksknsaat.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/grkozykql.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gnewyfbdz.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gphblassv.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gbjsbnabd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gdajwxyqk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gfmjbzxyq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gmyhgtwqv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gxvnuwawz.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gmtudblbj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gouosizoo.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpkeerqjk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gywqzsbjm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gmyhuqacb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/guwlfewcn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gffbxtxfh.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggdcrymhw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gizggsgqg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gggzfpvfb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghgxzvsxw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gilibgotg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzuczwasx.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gleaabbzj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/ggyqksiny.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggvtivpcx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gisrvbhpf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjwflnpzz.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gtavkpmco.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwmhgysrl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/ggfjwdinp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ggawvsqbr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/grqcbxhnw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gexqrqfhd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gnwjjmvwl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gtfaypbdt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gnaqdylne.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gonrtwrch.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdhskgbq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gropryncn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/glybayfht.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gqrkoukev.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gcdsbehtu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gxrgnqfon.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gnztvwvch.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/grxcjyiep.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghogetdxj.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gvncvsqcf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gykppoovn.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gtjwaxqyu.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gwdpcbwim.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/ggucgjqlk.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcnfdkvve.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gzqtstcsb.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gtpjhrbun.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gepwdoehr.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gtwqqouqz.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ggxrtivgl.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gbbmzodex.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gjumezxge.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gnlhkeabu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/geovehmha.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gorbqpvye.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gfhbezxnp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gdehuohlh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gdherjmnn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gffsxyydz.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gmoafranb.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/guvehlcyp.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/glchlcaau.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gubmsvova.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/giuwurqgr.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gcjfqvyxa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/goipmefiq.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gfcibtlyd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gcunedloc.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gqaynalsq.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gfotczbku.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gkyezcmrb.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/guogutdby.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gyawtwtjl.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gplrmuaim.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gzuxrwhod.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gnnajcbwf.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/ghjvyjzaw.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gcobxxkst.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gbknjpcas.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gykhhiqea.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbzyfmycr.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkfgyikty.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gfzmgioei.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gsfssvixm.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/ghmxlxins.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gyafhvkyp.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gfnlrstfk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/ghimfpogw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gxgnuyrlq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/grbvsixhv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gdwuejfxo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gucawibjf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gguxmghgp.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gnqlvlhib.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gdxubgnsr.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/ghjtzvdch.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gffxgijtz.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gzxkxqhpc.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gktywtacc.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gmrbdbupo.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/getstdhan.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gnbfusodx.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/ghvecmoqn.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gmajejimu.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gbqqamskz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/ghzkpzewl.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gmdjayscu.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gwfeykchk.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gishkkvve.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnekxbiws.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gfpynqael.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtfvaygfq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwnosyybp.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gddbhivzl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gbyxxeevs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gfpeyjygd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gdvckkglz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gjxezhvmf.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gvtohgbma.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gmszieaqx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gapktgrib.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gglxwyyld.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gdoaropde.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gykoufzub.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gewxkidwk.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/glqinhimt.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gmxcccpkg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gnsenpxxo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/grjfweznv.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gbelvhifj.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gzopwitsw.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gpeqbiiwv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gbdrkfezs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gjledtase.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gezhyefca.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gnaiifcxx.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gpsnmiklk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gcwhbdfqa.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gbuzxwvai.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gsykumyrp.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gpgooksxy.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/geowubduh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/ghwxvovdg.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/ghjhgijso.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gpeqwthqw.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjsqnyket.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gdubivkxg.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gavccivva.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gyewrqpjn.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gezwomoks.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gmxdsimfj.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/guvumyefe.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gqmwakspo.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/glgxjwnfc.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/guriidpta.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gukfcdcvh.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gwkconmxv.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gvfrcsmlg.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gvhryfmit.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gwwdfodbh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gapbxqsqt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gubhlmibd.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gdrvxodxu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gdbeciyhf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gtdkksbbe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gbmrrwwkx.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gtokbwhua.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gxktujwfu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gvdfnsrdr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/ggopdyznh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gliqgcwca.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gqvetkxmf.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/goyxvjmzb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gdrhngmel.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gmjiavneq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gnapokdnm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gkfzjiofo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gsaukvxms.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/goliakqml.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdlvlwlmv.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gvxytyngu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gtluaknhs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gfzklwszo.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gtexknyxn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gipdfiqpl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghpphiecm.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/ghfrvmhfo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvhblukel.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gxrcakiss.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/ggmqojdko.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gowwdrrfm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gqvsdsmyl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/geybsvyvt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gyqirerof.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/ggbweartl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gbvanxfaa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/ggsufjwof.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gtrgsgxgi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gmsglkurn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gahcbvsym.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gronrcggo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gatpqqfjv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gebwogzsh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gghtesanj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/ghznxrdwv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gimqbkpkz.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/glcvwrixi.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gjrkrsnoi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gwwcuvmhg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gumoptoni.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gwkjaclxw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/grupauupp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gxmafarmu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/ghurptlgv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gzybtgelx.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/grgutcmgu.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gpjnhmglp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gfriduvhk.sHtML


<!-- 参考信息 -->