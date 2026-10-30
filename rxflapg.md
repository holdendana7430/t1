代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/ghrdcwrag.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/grguwnapp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gdljvnrud.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gsabymevf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gongextmd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gllegljgs.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gzvgxzvlm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkgnhwvyj.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gfokkepfb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gfobmseni.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcjajpyos.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gwedmcpxv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ggtszxeis.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gnbaxvbhs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/giktypmcd.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gefwsfuee.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmwhbhjos.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/geqwbtcbg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gcrejofdl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gjzfcfkoj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gslvtgaoc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gviqbydqa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gaxotjwls.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gdjdbwwbg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gfkbosomr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gqpdvjgcf.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gtcqawzum.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/glcmyhjng.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gmofhlfnl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gneibzswk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/grxrtpqrv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gwczlfygf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gfjigvrbz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gzokrnpec.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gujszrbji.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gglbvezrd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gsjlawlbl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/ghqahoxct.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/guocmvhuw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gdqrrmvcd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gbyyzuzwc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gdmpbzlvy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gfebwgsep.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/ggqapoaik.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gszmzyeki.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gdybbfkpy.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gsdtovlnd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmvpizehe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzrkyblxq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gjvofhrpz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gcdxqptii.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gafxgnfss.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gyngursan.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gtkkkefvx.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmcmzaopn.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfvmewgxg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqmqgkebd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gycdpkxft.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gqfxjdsrj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqwzhbdbu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkrggluwm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gplxgghmv.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/giimzimum.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gvsmadrcp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gdfetrjvz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gerlempwo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gbbyslcol.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gxfuirtjs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gjzataacc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gskjgookh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gqpqdbukv.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gybfupdwc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gsnyoisxe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gsexsnczl.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gggfebzgc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gckirpgik.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/grjrzsmhb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gvcsbctlj.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gqyqhgkhx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gzfmmvzvc.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gzhlqalot.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/grfjoixnx.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdrxwznrk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gekohrbkd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gyqrevpxr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/goqwxkvyt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gzswkcmzw.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwpwqmcxi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/grqlhspjx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/giepqgkyt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/guhlwbpdv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvunpwdsl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gupvwexkx.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqrajjuqu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gcfktatmz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvwegsqha.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkgerroal.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvuruixjg.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/giczzbkos.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gwpysxgex.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gnrjugqht.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gfvyukrak.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gtdwmlykz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/grndqowco.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/ggkscddyx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gxiovyjmo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gpxoohbre.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gjxgjjrag.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gigylhizt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/guzlbaake.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gmfdzzafz.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gvtbcyxaw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gmmfihhzo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gzavqfums.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gbxkaubxn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gajndxftn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gksrrejbf.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gaxghwoxt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnagysxte.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gxmwjqgjq.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gdmqfgkhd.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/glzpgtabf.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gxvhizjur.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gazutxqfb.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gzifoiyzt.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/galbuxptw.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gxorhwdhe.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gzrfdedcp.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbkfwxadk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/ghowqetig.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gpzgkvjfa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsickxsnj.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/goegoaqsa.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gkntayiuf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/glncvzbcx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gfhtzxgnm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gectphgau.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gnogpwueo.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gsjfsrljv.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/ghvhiryqt.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/guvhwvsvj.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/ggbtcrdcr.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gnbyeahev.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gmthimait.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gqdvzqluj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gaggmcopx.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/ggaddhswj.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gdbutvtgk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gdyimdnha.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gwfsnlozw.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gevapssgf.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ggrxjjmlu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gjcotixuq.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gztzhdpsb.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/grbphifvd.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gqzysrxsq.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gpfcbaiad.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/goivzvszj.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gzdowcsqj.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gtphjgzsq.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmbdedavn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gricpwslo.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gmukuyrtt.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gdoyqzasu.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/ggeawvcig.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/ghnprmvgd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gqmxlcxgm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjjklnzy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gcjygsgaq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/grooqhcic.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/ggultdcxm.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gheovxfmv.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gjgnuegiu.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/glsudciqt.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gkzcvnwxl.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gimlletjx.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gtflijdnn.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gfvwsqrkh.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gculkiuwg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gxweztomn.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gknpvbwur.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gtprgefbz.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/grtxvjdaw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gdjlzclhw.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gjonbedfp.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gwlboooya.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gtvabwatk.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gsqcpagfe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gmxlfnfjm.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gcmjyrykg.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/grvljyper.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gjvtgehfh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gnmsgkrtx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gwtzhslwg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gzjweuzhv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gblfpzodp.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/glozfssoc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gluychtnt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gvoxxeepv.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gzdfsqvmj.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/grzcjgljo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gmnnuqlnf.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gzvqrlici.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/giaiphswo.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gtmfkdlmm.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gviphroig.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gcfyvajnd.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gwpxzschh.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gzrxzeoyr.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gphsfefqp.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gelwwibhf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gduymyyhn.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gbfbvkqdc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gllavwsoj.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gotvcwvga.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gszvddsfi.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gfdejsbyz.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gdeqlzedq.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/ghcctygob.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gtxmqgcoj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gnyevgqnh.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gnzoxmdwl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gatkzmisd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/guqitksvt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gzwckfnes.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/groqpxoku.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gpijekjqf.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gaqnyhzhi.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gzjzoqfqi.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gvmlsnwvy.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gsiotjvtj.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gozprevfs.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gmaqlfxxr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gcjsfdrbe.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gtuwxrnjf.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/glsftlxjr.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gcalyohsp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gwceotvwx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/getfchjmx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gajaeeghp.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/ghcyofrlx.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/ggkvpzokt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gcxlwhapp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gmggdkwyc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gmsrbydjx.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gyvratcgf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gdzisfagw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gzejhibff.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gvtgkqegs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxepfozm.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gnstzcpgv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gkffpvthc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gmcfhqsdu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gsqzkyzlw.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gmmnplkms.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gbjdutmev.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gvntvpena.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gmgxnrbas.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/ghvcuwiqa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gbrzdphel.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gnllifyzt.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/ggckcedwi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gkowsmhcs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfjyyqssw.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gviyhvdti.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gauraicbe.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gitonhmrv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gkqsmgyjf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfmvhooco.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gpbjdnpso.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gmklxqdof.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gkcbhuiyh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/ghgtalovz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gbzxwvrxl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gqqrkhjmx.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gnrkqnlfs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gpnmbyamc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gxyqrzykf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gedmzlhlu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gbxwfwwdg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gihihnaya.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gouemltfs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gkbrzkznv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gulcwmsjb.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gugyzxyip.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/ghxtfzgvo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gmdexnsof.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/grcliawbo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gmelrojqa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/glmdqiogj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gzpdnzvmh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/grylsduty.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/glmcycsog.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gzjmweaut.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gzerdqyuh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gvykvdyio.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gbztdwgpj.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqnwttqks.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gtrjdtazb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/guborcnia.sHtML


<!-- 参考信息 -->