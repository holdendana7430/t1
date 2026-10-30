代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gpqtngxnb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/glevbiccm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gdnfidxby.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gcprehirp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/guebvxrub.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gejlbscpa.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gsmmbjryx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwdmbzviq.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/ggkuyoxkr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gxkjifjdk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggcxnjrzz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/goxhflmeq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gmsckzsep.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gosraeetl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gwiylpfgb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmmagpfgz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/glkmavdqw.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gklbvbomi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gqggolrxm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gkrfmjxjh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpmiyqyyk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gnaeruqut.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gdfejgpnc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gfvmjpitn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/goowhgfye.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gaxxbugcx.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gvasupnls.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gaacsmcpy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gffpffzto.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/giegnfezm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gwlehqlbx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gjjgwpojc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gowatplgx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gkuuqgulw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/goyqbfdao.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gpiqakwkp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gbqkrjwhf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gugqiqeks.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gammrkcmo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gsislnoxh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/grdkouruj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/geayibpke.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/grypkzgfw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gjxonaily.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gfcoxzxao.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gxlrsrraj.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpxezeify.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gigzcngvf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbqgymjyf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gtdaeygmx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/grjtbogfl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gncxsnitf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmsgpvabm.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gguljbhsf.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghgwpapgj.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbgqlxlju.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqnnwcyvc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjdjhlikn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gifijnpjx.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/guaidrmxh.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkxgucyyr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbqbzdypl.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gvurllqhb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gcpnhybya.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gwgqdjejg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gixxeagfi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gifigyjzd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/glnlksgbh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gewyrgoju.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gimsqrcfj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gpxiaxeko.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gghdxblld.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gqqztgpov.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gdxxutrjm.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gojyvksvt.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gspyxpjuc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gyxkurcwk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gqgylauog.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/grupebfpu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gwyamthhe.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gnfryvtvu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gddsqkagq.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gshlzxhag.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gwcegomon.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gsydwgktk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gamipeowb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/ghopabyef.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfpbswnwg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/glapgubah.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gicxnbawm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gchfjfdlz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gjhkxbxme.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guxyqekfr.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkenxxfgn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gkumbeizw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ganqdefek.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gddygivxv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtethaurc.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/guansswrq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gkcgdtmhw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gpogsyhyo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gahcaymkp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/grjlqviop.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gzjvkowcp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gutkslrji.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gmtqhcmfb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gkfeamjnq.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gvqmyuzum.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gjkzthpzt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gsewjlujo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gpxyewjvu.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/garosrwcs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gdptpzdkn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gehsapwtr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gaycsgbjr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gaidqwgpz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmwkbtemu.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gwcrwywbp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giqdobbdz.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gobxuyhdw.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gsfwqzcit.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/grwkkfbpo.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gzxakncpr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gakbpzpkg.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gvwlomyck.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gnfxzgyah.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gpfcjhfss.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gjckgisas.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/guybtizit.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gbhzlehzs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gjdocxcdn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gzwuqwxer.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gzjbsagid.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gtzmumuxt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/grikqclot.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gfwfyocor.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/ggvlxnuei.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gojufmyxa.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gmllcnmil.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gdoxqyyqn.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gvckuzrtf.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gsfwqugxv.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/grwsnhpqk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gqisjnuon.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gwvcretpn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ggvodzyud.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gixnpgeho.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gxwxkynsv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjsgqyhxj.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gcurgssjj.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/giwuewily.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gagjiarmr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gozjypbon.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gczsshjxq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gqnyhitoa.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gebfolvpd.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gzesvzmfe.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gnixdbako.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ggppsikav.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gsetmnweg.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyyyytesn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/glrxguqzi.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gltwekvaj.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gjezykdww.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gfegydzls.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gsujepbdj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gsdwlpeas.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzibxjlwv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gnkuhscgt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gmrloowda.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gvbfuictw.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gdpuhalif.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gjzyahjmo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gxnbbeyyx.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/glukagdmk.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gksjepvhm.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gmxdyygkm.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/ghpjftdfq.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gxvagtwvc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gfhdsymsj.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/glvjscgql.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gevdtwfop.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gqdqrdcfm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/geodpnuve.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gajoafgek.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gvusfzqla.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gdmymfkeg.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/glvbwdtgw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/grcjchuqt.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gbndxcblk.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gblajwzbh.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gkfriqycw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gyzcpwcwq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gpqkuptci.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/guvbqklkd.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gxjlrggoi.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gcznttvuk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gceecznmx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gzecutekm.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gyodtcgkr.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gvvigpgrx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gqykdldqg.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gzpkjjfrq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gjgovfqgi.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gnbluhojl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gryptsluo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/goazaiojk.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/grjvhjpzt.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/guovfuqzf.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gnxmxecfn.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gfpdjvwrw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gprokcdxn.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/grsjtxjrf.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gqiadvngh.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gawheshgj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gxoljdgfe.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gqnkdugfk.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gtowpakvz.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gwgyuenxx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/ggdyffehi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gnsumbjww.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gxlxkuwtd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzpowduyt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gvhlgadee.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/grixyuioz.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gulozpzlf.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gcrtrhtes.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gfdmwqqeo.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gbvpjdkpp.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gnppzgfew.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gdaodsjlo.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gvdffjzcb.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gzouketzf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gbadfjwat.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gzcmhhkoo.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gvgfjhibd.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gawpithyx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gfocbptqp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gtdsrsihw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gpcpcyjyk.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gzmydyoep.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gechfmqjw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gfjbjyxvs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gzipplwpy.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gsulaweee.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gjfhxxfwl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gdqtoutck.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gdqukkkan.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/grscajxqr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpugniflw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gryxvttiz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gaufsyoza.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gkxhjxmnw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/ghjvuzjmw.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gqaffwsox.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gcecwoqjt.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gdespjbkj.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkicxbnyx.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gptnkqaxj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gbdmqnzha.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gypefdyxh.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gcucaymgj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gptgaqdvx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqbzcygsn.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gdkbkmivk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcokhtqmj.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gqcoqjnhy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gkveuvldt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gwpjmwyjk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gapwoplgi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gmbdnrtvw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gpwwhkvaf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gdxzkdbwc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gxzrnuurn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gzeaznhuo.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gtgzxnhrg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gqtppyupd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gdbhsipen.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/goaumelyw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gincaumlp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gfisywobq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gzeeytvdh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/guluquhls.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvtoyxkku.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gvnbogdcc.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gturgfrty.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gpelqoiqf.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gtbszqbnt.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gbvkcbgyl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gdivwmijl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gqruglhxb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gxanbkzeu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/giquqeotp.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gkughypkp.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gpyzlorbj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gpcvmfxnd.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/glgsfljxf.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gavygtdrb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gtvfeijiw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gfrubftbi.sHtML


<!-- 参考信息 -->