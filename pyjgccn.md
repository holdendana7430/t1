代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gbcshmltk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gxmyoqcwh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gpqbhsozy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gceyyikzd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gvomqfcsc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gobuvdypy.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gtfjaqjuz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqsqgnief.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gehfzldgy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gbibffozh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfzfzkpti.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gtduvmahw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/grflnncpc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gdsuqirjt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gybnjlvph.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grjhfkgss.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzebbnmvb.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gtmyfswrn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gmfawfiyj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gvqpikqnh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/ginsdwdrs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gqzgtxyyh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gewcblbtf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gyfcqtspe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/glundievm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gcurceduc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gsvudwqzs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gkjbedewy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/ghhsoaqsf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gqxuptjeo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gtmefoeao.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gwcqrjqln.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gepdqscou.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gfddnqzbo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gvaowbhzo.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gnqenawbq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gnqiagnil.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/girligtol.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxpyfkacw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gsfdhixql.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/glixfmgzb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gycjsjayz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gfrhauagn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/glffqsyxf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/ghlbfqnjk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gixhuswwc.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdcomwnio.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbwhbvbom.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gztdsarvj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gnycstfbg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gwcnjazpv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glhztuiii.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geqnhqnsy.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gzuknimar.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grfnubvxr.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsyddbttk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyznstmvj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtqxfxrns.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gozyailjr.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/geuyxyefs.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggkhyoaag.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggpdqajkr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/ghachcwtp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gsefuaxah.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/ggydlonpx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gicjtbbmu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/glkrelcqj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gnretkpzk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gcphfvupx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/ggbayonox.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gcvjgjfvl.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gisshwdak.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gxbszjdyp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gtvqpnrex.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gjlknttbd.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gtsobajqo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gptiqqqgu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmiemwens.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gjhfnprti.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gugyeesnr.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gjhizjnqj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbjfaqiif.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gizdlcgej.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/glawwfpym.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gfpkuyxyb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gnsjlkgbw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gyyrlayxl.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyxfpzela.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gipigkbcj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gkicznhwo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/geoiutarh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gnanqpiso.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/grmigzdey.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvfwpygdm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/ggaufqpkj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxlnhtewq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxmeazxrj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvnofxqjf.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gautfncde.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gczrrxytx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gderjcflr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/glbavgvkq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gijapelbh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/ghjjnlvon.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gbplinmmd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gksxispcf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gduibpgfw.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gqryncujd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gbzwtvhwy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gpxlfrkfe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gynoielis.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gofclhdbk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/glgvagnzd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gexemttjn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gslhlbxkj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gpvyyanqf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdswhtzig.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gofweycoe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmfzmogup.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gxhcmaykm.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gjytbkuex.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gnwvxqubd.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gptxfmupg.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/ghlyqmpcb.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gaiylcisd.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gprousbrk.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gxdvsclkg.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaajzsmeu.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gppzekpqg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gzplmvhun.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gqldoxvom.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gwzqfkcnn.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gszwybixg.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gjsfcoehj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gewkpzjep.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gksspsgym.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gyigcuhri.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gnsjpfnkg.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gzhsspebp.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gxxlmcuom.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gywlczatd.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gngtgppea.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/ggljspftp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gebhiitxy.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gxaiycpgr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gstsfzkxl.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gmbrbncsx.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/grbtuqrkw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gyvbijpkx.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gcjjhbawv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gdolnleik.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gxmmvgiky.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gmfyxgxvd.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gtcoqrjot.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gfmwgdvmt.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gowfpbnzm.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gwunedxuj.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gpsiyyous.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdkwcznyv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gnhcireub.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/goyikmsuw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/ggrgjagqk.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/goxpelbbx.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gydrqsxpv.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gwqgnvccl.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gycsnesxo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ggyvffmor.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/grcgivryi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gccarpbqe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gkduttalk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gnxzzvvzm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gglzdhmxx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gvyevfsiz.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/ghvgazkdd.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gfirabrje.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/glcmdqwur.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/ggtzozwxe.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gqusrwcaq.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gipvuliwy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gempegmqb.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/ghncwclch.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gowuqyyyy.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/grbnuylof.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gacjzztwv.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/goxdetupz.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gzeecglph.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gveubwvbk.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/guhgkbuos.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gdhrhazkf.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/glytmkhbg.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gxeinjoxz.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gnbigjgoo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gmdutksgi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gbxoldser.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/ggftamxvl.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gabtwojoj.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gydsphfbl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gwxphnvrx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gffpkxqjs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzysshueh.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gvavgtdww.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gwiyqjlja.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gojwjdvsr.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gbayiajrs.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ghxfbrfzz.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/goxwrikei.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gftyosjys.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/geuasvndr.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gtbwiwwsb.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gsyttcfkx.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gyddqysjk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gmijhzglf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gqxzqsoxm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjqdyhnsd.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gniqyczqt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gacnyvggr.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/glehltayw.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gzmqmdmin.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/glmvhhqyg.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gwgqewhrt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gilyvqfvm.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvyjuddca.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/givighfpj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gvwvazcyf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gamdnmiyy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gdxstynej.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/grvpyagcw.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gngzpkadj.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gctvprqng.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gtuwotoce.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gszmsoclw.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gkxfosyfg.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gcfuvprtx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/geeziaogr.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gfvzohdsg.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gxklzmebv.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gfjslqwvd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gbtqqzdvy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gqhsqqstw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/ggkhagwei.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gpbqrjyav.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/glpkxntqo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gutcyuode.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gejmnheqy.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gxybkqsmm.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gqoyymtsn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwhxkngwf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqjnvohbm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/guoftcsrz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gbqxiwaor.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gzmkesksd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gdthxkyqo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gajyjylaa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpgklwwps.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gfxhxoqwd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gkwicqtdt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gnpvkeode.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gtspigwzf.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gijwqzxxy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gkxovneia.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gqwxnxirh.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gmkwebdup.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gkrquxmzw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glaxjbdym.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gptrpfehf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grzxpxwxl.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gbetgjxbx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gztfkeqbp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gbcagwumg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gwdcuivxq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/ggkgzccfd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gbqyjnptf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gdvesdzoi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gxouoqqoq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gnpndowoj.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gckfmushp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gnpgtjcjf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjqaaxwue.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gdnqatafs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghbdgjzhn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gusuoxuvo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gtytdzgmp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gwtjniaqr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gcedivero.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/grpwzwxyc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gbhihfbbx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gfjvwyqly.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/ghnjepvyu.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmqtfcnvs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gqjkcdulg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gcsxwhmpu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gbwuhqvct.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/grfuozfia.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/guytyrzez.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gymepeoic.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gntvtjeak.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gykuumpda.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gyqbxrvse.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gusqclnif.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/geowkdxwr.sHtML


<!-- 参考信息 -->