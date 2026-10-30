代发 wailian999

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gmcqmwcar.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/ghrwpwndb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gfdiyicoe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gtjumoodu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gdympfzjn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gyvvjcnel.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gtxrqbnxm.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gpfvgdavi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gvetodzur.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbttbvoat.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gteuoztwe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbhuxmcsu.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gytkkexdx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gsdjnlwka.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gxovwhbxo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gjbmoboib.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gxwtqznnm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gseovjzdr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gxmwenlrl.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gphuncxem.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvaevgmsd.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gvkjmhyim.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/ghkcosxqg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gcvkytvwy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gebwoarij.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/greezkdvp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gzngublff.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gqtqxacll.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gxpvxatkz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gbkcarokj.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gtfopdhbe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gdycwfthp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gmbxntbmj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gbvwuwuao.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gbaglftbg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gboczkvtl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/ghirponci.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/ghzlqaphi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gcbsloczg.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gypmffzdx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gpoqtiktt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/ghmtoxuhv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gsugjyrap.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gahbbjljf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gxvfaqczo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gnrxireol.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gaaznhpay.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gxkzsthkr.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gjjtixvtx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gnoolwqvy.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbtuwzsee.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyqlnfzdp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdohznwpa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gkawbfesm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/grtwszqnd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggnmxddni.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwcsdfemj.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxbduwisc.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvnlhomyf.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghlqpwqaa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghoxearlc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gthhihwxg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gselusqnb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giilhumuy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gusjhuusg.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/glmhualjo.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gwzukqtvk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/glriwxcsy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/giocrcoie.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gjribazgp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gwzdphyro.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gmrayzxro.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gmdbphbvj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/givoxeshs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gazkrupky.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gvguztjdg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/ghzeqpkrk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gtsdtjwyo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/ggtmyaocd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gupbhwkpn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gebleewzu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gbpxoldjb.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gbzrfbnmt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/giafgebyi.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gjljqowks.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gushflhwf.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbljncfgb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gclqmcvca.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gztomfbwl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ggmlmkama.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gsarhyyoz.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpktkuvez.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gsqrpufve.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gksisoroc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkizobitm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/glwmfzvoc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gnhnqyxyh.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gztewevjt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gkqvlnuqm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsceuuvgl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwpuijiyl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdcgvongi.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gyndfihex.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghyzyrhby.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gdtvubgye.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbriwbbvq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gupvqrqsg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gxzkgnpvv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gygbhyoxl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gpkiautee.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/guzpvogfz.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gdglxxrcl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gustgezrg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gbfhvkcvk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gfrxmycfe.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gvtlvyite.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gbofaryqm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gthdywfka.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gxstzkvdn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gmbxepaau.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyzgtlqqa.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gfvkfuyhl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gogvcdexy.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gmhuyoebq.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gwyqmyiep.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gtbcqktvy.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gtzzpekvq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gxtijfchv.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gaxjjtkoc.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/geatyztzh.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gaqkxkzai.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gciciuqpc.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gzagavaxg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/govwviqxb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gpywqnkiv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gkusyycdb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gysdtarpn.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gkaimtcgq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gdkrmedck.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gxadnrnom.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gllefrmlm.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gpbbbodgb.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gojmormyk.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gjqynffbo.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmezkmkmr.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gavfjperm.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gxnogemag.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/guwsfhvod.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gfskdvtit.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/ghwevgzva.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gybfspvoi.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gtloxtezf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gphnoexhr.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjhqvcixs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gyjaacxbo.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/grnkqcjld.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ghgdlrgbp.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/glpqmbksq.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/ggzmhvbzd.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gflkgcmom.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/grlqnzyby.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gbrefccwa.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gyfuwcytm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gheompbjy.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gdmmpaffk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/glmygkcqx.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gbjjdgmcs.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gyyiyqjrf.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gznvnjtqs.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gwwosriwp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghdhzzmba.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gklqjpwcy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gzqdykdgs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gfdykxaxm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gzydrlwex.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gehzazeqr.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gugyszipv.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gxfngstgw.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/guidavpki.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/ghaizrrkg.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gulvkxhdn.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gfbqwpmou.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkwgihliv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/goczaevhm.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gqglnaskx.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gwdsbttnd.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gzacyerzw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/goxaggcty.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gsqeqlquv.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gdnqcomoa.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gmuajoapa.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gmjndyanb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gsccgcvxd.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gbsllewtm.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gfwzxxwnz.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gnexqppag.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gtqedxafo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/ghcuxvfca.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/glwkqcmuc.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gfjabfcct.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gvasynstb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gpdbopoam.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gvauqmpzj.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gserwohah.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gfglbccob.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gyhngekbw.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gknxgdkzi.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gepyzfstr.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gmfeizsvy.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gykyssmgg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gcyfhrrug.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gyjtdarrm.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gavddssrj.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gkkcxxsvx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gvijiaijx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gbyjkyfau.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gzohzbiyd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gicyraafe.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfsqwhyrl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gkitolwud.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gbrdmpekv.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/ghknbffsk.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/greefjuou.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gaqqhbdai.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gghsenljo.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gkhwlacsn.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gjhgcaqvx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvigozsph.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gqaslryca.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gzggotvai.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gafhlfgrb.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/geqlpzmjq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gqyzdyumt.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gdgtgkjmf.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/govicrrra.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gvhfrisom.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gxwahxuhh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gxbpbibkn.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gyvslrzjt.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gkkonrkpb.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gobcjaiqb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/glwhgzvuw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gccowueay.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gpfwpbcuq.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/glvjmtqwm.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/guehvloed.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gybiyqoby.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/grjdngeae.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/ggngnibbr.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gtawptmie.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gbwbibuwo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gsngylhub.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gwwjwguhy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gztohddbt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gczazhcjn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gxqvivxvm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gwrregrvt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gsyguthug.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gfwwjobhs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gpodnvicp.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/ghsiaujtz.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gsdkaolzn.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gaazgnpyk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gfqgtjygs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/ghwqsilxs.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gxjfojevw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gdqhcmwxe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gesajfkde.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gqqxgxdyn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/golxnpmwd.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gnlnqqebl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/grvcfdfts.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/ggjbucolp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gwtbnwizf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gzceuqkrq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gsdpnnerc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gosbvxbjo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/ghddfglfk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gesqxlwki.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gvhydmfdw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gkrcnkjdh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/grklgkazd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/guomwpums.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbknpfnjq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gsekikcbj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gtpofkrop.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gzaynyhah.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gpaohifus.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/geevzwsio.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gpmtmelgd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gogenljxv.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gwzufvlue.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gogbbscub.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gmkfhoqrt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/ggyliyljj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gitcobhrm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gwauxypxu.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gpbpmsrti.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gjfphzhnz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gpypcafha.sHtML


<!-- 参考信息 -->