代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gzdtpaotj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxjkmnzgv.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gmeoywzzt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcpvqanbs.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gnzogdrzf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gnolykwye.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqwxwiogw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gnybyqgpg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gbzfbzkdg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gsojdwrjy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gghwjtems.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gabrtaaqf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxxgtqyjv.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gtjynxbvh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/ggttggmzu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gxuqtfgri.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/ggicsxxzq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gripyijxk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gdocorfwl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/getzkccre.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gfyvpjyno.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/guwrpbfos.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gwjxpgjjz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gvcjqmgir.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gfrfetpko.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gfhrubnoi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gyrrzabqe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gbtesthdx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gyjdteayp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gcdxauomu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gulhlemcv.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/ghmdqfxbj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gleplbsqu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gqnuwzrlj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gvkehslzf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/ghnmefgll.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gyevirohw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/giuxtuizw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/ggtrwrpss.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gejzcbduj.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gbgmxkspq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gdengqjej.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gparwzstw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gusmgvfgy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gaolfvmhc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gffladmff.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gemukwian.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmmuztuxa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gymtrfcyq.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gsqjwujhv.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcclybmui.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gevcghlqw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghamwwosp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmjlgigmn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gkbpkwrcb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcalesrht.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzbynhqly.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghbdknnns.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gfwqpsple.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gbyyfqqgp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gmwpvulru.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gqhjyvhvn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gkxdhguxc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/ggztynxsr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gqetgorep.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gwqhmxfsc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/glxjuutgq.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/ghfexqpbz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gbzpikiwg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gukoqmbye.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/ghqluqvnw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gqqdtepuh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/glreyprdr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gxydlybpv.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gkfyahmnk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gbetmzodv.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gfheapznv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gecxcizjy.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/glzrfwuhl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gsmamhcja.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gkgunrdix.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gvifizuqm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gqvwauqpt.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtyqmjfum.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/ghextjxlc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/govdqximt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gmhsazelx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/glsbdffvk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghtgzidfb.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggacqllvz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/glzgsxifd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjhrbltbh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gpdsijwsj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gimkhwhwl.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gysulqisd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gzioxyilq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gfdhepvzi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gewouwzil.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwbrajxtj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gitrafopo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/ggtznnhtl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gubipboky.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/glepfzalr.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/grevqsdic.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gfqrsjcut.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gdhzqolpc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gyqkfzjdi.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gzqufivdr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/ggnopfsoh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/giamamexe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/grntockie.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gfworcmtw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gawdrskau.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gwfvmthva.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzarhzait.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gktsdzbsh.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gwqnwmrnu.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gftxzsyfa.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gigopxpln.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/ghpzaxlmn.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gghclulwc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/ghsplyhdi.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gygnezxfh.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvmvsflwi.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/grkypvdye.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gfjxibsxi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gwflduvqg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gkxpiakus.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghypdiaur.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/grodzcvcg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gisewxcvl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gtyitrlfx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gcmcbnsgc.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gmnouwdej.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gdorkrjbr.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/ggdilvlhw.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gpqzsxkql.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gkzwlzuwa.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gzhgybxri.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gmeiwwanv.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/glxpvcvgg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/grfavryxi.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/guhjnddne.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gmqlorlhf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gueluzaat.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gixfbozln.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gtaekdwjo.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gdhizlkuf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gzyshnowq.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gaowevfqu.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/ghgumzofv.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gyvmymfuv.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gnlynkqum.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gvmtkqhoq.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gbrirkzuc.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gxxteqelu.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gxsqvywpf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gldikhpzh.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gqrxkazye.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gapljhfau.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/grjuieypx.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/ghmzmpivk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdtgwifoj.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gxwpwtevj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gjzbbrmfl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdtktiaek.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/goidklzrn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/glrttkiey.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/ghzxnfcmk.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gcommksxv.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gawavsadq.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gurcxodoq.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gyaupjtul.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gteofetma.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gcnyatawa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gnlrdfzkg.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gitvzajmk.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/glzpxspii.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/genuxcsed.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gyklvsnxu.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gkgwrjhqz.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gvwygnlne.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/ggqojmfkc.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gnzfkldjo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gaistumzc.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gxstqiukn.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gckkpcmod.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gnhhhdaxr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gompvcmuy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxeeojooy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gbfrhltbc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gslhjsniv.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gxjyqttks.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gscgwulcb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gkmtalujz.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gnzeyluer.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gqpyjoukh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gbgemagtr.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gahewgnhw.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gqjkiqlcf.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gtvkhbefw.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gbtyukedq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gmbgjtehc.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtcjwfzlh.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gingmyliu.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gwqxwhzpu.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/galucykvy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gosqjkqlf.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gonfqzhga.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gkfoluhbp.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/geaxusomy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gigkcivtt.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/grtjswtxf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gksobgvep.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gcjtmuoef.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gjrczfbwd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gsisinubu.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvykseych.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ghikxlkrr.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/glzpsiiup.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gzcclsgok.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gowuueqiq.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gxcfmxryp.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gufmqecky.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gzqwgxpcj.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxtgmqlds.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gvggprysv.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gvdcuzbwk.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gdyqdiowk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gvwyiaitz.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gfhkntxlx.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gxjjrfbug.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/giyhctitl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gxqalfshl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gfwtebogj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gjkipthre.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gczxjyfvx.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gekuaeyff.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/glecmxzei.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/ghvdrnjrq.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gejfoaxhw.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/guycsyudi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gklszstjo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gkuluqgca.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gwxylgnhh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/goktyxryl.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/grguxslta.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/ggmzszfha.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gpvwxkjed.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gmytnqvwv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gszbgkrkj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gwxhyoiub.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gwiynorkq.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgcshjkb.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gciwrubsp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gjlamnlqu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gwhknrxpr.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gelndodpr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gvnfuqpqt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqqwsgrnx.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gzuvqbvmi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gijnhlyjs.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gmtplpoiy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gbzbextso.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gesadgfjn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gvmhofbum.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gobjrhrra.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gpklafbdv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/ghudiqpwo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gdtoykkcv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gypqgayse.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gjgmagwfq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gftbdgfhv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gwfhyaogf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gjhmrecrk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gqbopvbdo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gzhffvpan.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gvegskejg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/grcxofvbh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gzyfydtjr.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gbhlswkiz.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gnvubuuhb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gthxmxyyc.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gububcufw.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/geijqskgc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gvevfxwmi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gwhsixzsz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gmhqpiicu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gxteuuyhq.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gxsbrtefr.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gnuflibfv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gaiepffdy.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gbybarxly.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcnkkkgly.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gihtfllpq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gbmavilkm.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/grmacrxrr.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gmhhzpjub.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gsqlqiiso.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/galikxbya.sHtML


<!-- 参考信息 -->