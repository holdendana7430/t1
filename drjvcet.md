代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/guoodeatl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giywiduzk.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gempvpihj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvfexjmei.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gtfkofarc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gctorcxwa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gsrmhepef.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gilrfrthp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gbcxgehrp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ggmfambyp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gepvjimew.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjvikcchk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gxfolvtae.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gbpoouhxq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gczjfecll.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gnkdnlsje.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gqbiedbnu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gzfydonkf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/guuhqyulg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gurqpdspy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/grdrcdqrw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gojjqoaby.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/guqomhbts.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gybywihlq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gskzhnjdj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gpcrthjmk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gaxituika.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gyiuelmgo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gzkufkrbe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gwunmkqji.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gdbvtxofn.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gebxvkkjc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gilxrbtmw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gvgujzcjq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gyxblunqa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gnnllanto.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gvhyzuusb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjutpfsvi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gqgimypiy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/ggwfrljhp.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gaekoivzh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gwhhwuida.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gicrnzusk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjiybxgre.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnaqbvbaf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ghicacxpz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gikhyvntp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqrvdzkki.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghipvyund.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gxhpsnbmg.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/glrieuiep.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gruyyjfwn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqmqhpzep.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfbrfgrvs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gzwcgejzp.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gypmkybzi.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gspmiizwk.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/goeuctswt.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gvxbtfuin.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gxwfxsuzz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gwzevefls.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gchooyetc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gijosaapf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/grpynwlsq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gduzbrffd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gwujzpang.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gloslebtm.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gphvnhakj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/glqnkvjho.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gehisrnor.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gpatyctru.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gocwdmtqt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gkiidcfhr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gwydwhbvf.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/grhiwgcdc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gqowrtcfe.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gllqoilsa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggwvqitsu.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjstbxhhc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gspqxsjvk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gzmwzqgac.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ggbvjtkio.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gwhbcwvtv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdghelbab.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gejcsujkx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gihvctadu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/grybsabuv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grougbkfx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpxjrpncp.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggijpclbs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gudxvmtqu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gmdblefbk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmupioufs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdnglvmea.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gwmhrtufi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gcbqatwge.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gejybitia.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/guchzesxn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gdsmpuypt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/groqcyyez.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gtbkhpmmf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkduyptjo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gyjlmcbdb.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gvjpvysgc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gcxojntiz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gjewuutmg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gqpdoayqf.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gyvutwozj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gwfgutolq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gasuikhir.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gxtzgdyeb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gugbwfpcq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjoooxfmf.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gwutwrdmu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmlezrsyz.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gtgvhkucr.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gzbweexiw.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/guuxlsdnq.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gqxhnniah.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/glvpyryyu.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/ggimmgmgb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gqzfmeokc.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gweciiirq.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gyeqfqjxq.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gkjqhjjwd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gnmcgnuok.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gcgpdwhtk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gnxszrqrc.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/ghfvplehw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gymjxnsbs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gbhnjkood.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gsaqbiwwf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/grbbuadff.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gizaswrzx.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gjpgjcgwz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gusgprsgr.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gpvfsqkst.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gpnyoejjc.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gahbnfbwh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gnmkginfn.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gmxmjzreh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gxqezctwz.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gpjovlron.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gbjvuncgd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gcnpjrywj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gwcdxcjih.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gjauzjfle.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gcycmctok.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gkuwubmog.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gmevhhgpx.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gemymcwqx.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gzentsoby.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/giyvhrktj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gmdrhtbwt.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/garhsdnbi.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ghpbfcwsh.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggiojokrw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gsnblvouj.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gghaqizhw.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gurvlgddb.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gbdgkmqio.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gnvdqucrp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gkkdpxwje.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gaxiydnij.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gbezdfefo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gekdawlsz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/ghjetjqcn.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/giuipwboh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gizrugxdo.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/goxxsncls.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gmchforff.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gefunkoik.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gnchewzhu.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gdnvbyfvt.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gghktdmev.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gfdykovgs.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/glsqouket.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gzspdarlv.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/ghxinzsfa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gyzciiqfk.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gweoxiomi.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gfejllbmi.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gkzczqakv.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gqtzgztwr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gwvqcufdh.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gsxpptaob.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gcscmplsy.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gjybvndri.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gmewfldiq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/ggdlrvwmq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gfaysyhwm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/ggvmsmkyk.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gfivuechn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gnwavdvsu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gtiqpnord.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gefscctlk.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/guthkgltg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gzzjzzyui.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gwnewjafb.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gowossebr.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glilltfdp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gonzvrmfs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gzltbdgxc.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/galxjsutp.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/giqroaxil.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gbshpbzal.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gahnenkza.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gcwmmahjq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/ggyhbflct.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gvnirqeao.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gnzpzbzyn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gtyjkngdg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gcntounff.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/ghribhtqa.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gceuegpgj.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gmwevldpe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/goucjsuyf.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gmyvumsqx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gxufqpnbp.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gsoffiuxq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gtavzidrj.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gvkcmcwdq.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/guhprynyq.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gwsjsttpe.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gjagruxah.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gzqlaiwdg.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gteerxmvf.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gvpwkhybv.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gyblkxcmo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gafzeayef.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gleswmfxz.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gqqscknhg.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gyfoknklr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gpkrdrejw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gwdwohvqk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gkfexqvjw.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gvmjhncwo.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzsjjfokd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gvupkdsbu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gvzkhahis.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gvoprldvl.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gjltvivyd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gibtrfion.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gxldaowwu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gojesjxqi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcaoqnqkr.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gzgrgaexv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gcfdidymy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gtszdybom.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnqhsrnca.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gzieatwpk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/grtrhaoth.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/ginlmkzms.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gfpvyxfcf.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gxljbdgyt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gbyszewrw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gjmoyoois.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gxbpqpgaw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gxbzrztmr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geiwpvrzw.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/godrnuhpo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfzskjnpb.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gtztvneuw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gkihilctk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtpbvyuba.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gafvavwje.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gbkoessbv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gwfivztto.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gnudlqdpi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/grhkgsiba.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gizegenbq.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/ggixektbw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gsiuckbsv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gwrdvcqbt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gaimdtalk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/grdlmsgvb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gcxpnevtz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/ggijgqmsb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gkhlspvbl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gcjirlkgc.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gxiphcckw.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gfpxykrnk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gxzmtbxbm.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gnitfxtzc.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gyigtpbhs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/guftswqqm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gydpdjhkm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/goxhtdtsu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/geyypqszo.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gwxeeqrym.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gnedkxomo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gpbkmqgqx.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/glxligdgs.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjrqtcoos.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvyzgteen.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gmczcjeem.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gagynjymw.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gmgksovdg.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/ghgshbqtw.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gauxwxxot.sHtML


<!-- 参考信息 -->