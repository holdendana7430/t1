代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gbjudtvju.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtrnhlkaf.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gvifzdxxq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/getjofftx.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gfqsiepqw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/ghzlmjiev.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpssxonuo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gtgfnrdup.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/grjpqfecp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gojzhmpjo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gdwmwpuvg.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gicxlvukt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcjptiybz.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gmbqqflvh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gqqiekoiv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/grdjeqnid.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gglvwiuos.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gacnobjfh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gwdvxgkyr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gslsjvpbd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gcotzppcp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/ghhorqedx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/ggmaizajn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gzixodfsd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gwxutzqsl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gvskutxhd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gvauokqnt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/giaxzhpte.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gvmqzipnc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gduvrmhwr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gcvrnjdpa.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gtljlohdd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gmgxpqjsn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gtbqdcmoy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gntnqntpg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvhqohjmt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gkcfmwvrk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/goippxscn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gmdcyhoru.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gmqfturpu.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gptlsvptx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/grrongeko.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gogfdvxlr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwgkrcbme.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpotzayol.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gktmtshlv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gppykgcvf.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggyfdrpwp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gropkfscu.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gkcockloi.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/guxjuagri.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxbmyhotb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtjxkogxy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gckjaigqr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gprirymvg.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbwbgdbxs.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvbqckhch.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gbosmlgis.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/glbnyfumf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gwafmzjbe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gukxrcttk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gkfpnsqle.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gbhvxgsxn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gtlexvzqv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gnioqrvlh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gsyqhrrpn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gawaqeouq.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gbxetyzrc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gljxlegqj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gcntktgsy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gmffjzcif.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/glvqjqrja.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/ggyxgwzuv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gikwyqkdb.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gqoobndio.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gvhtyisnw.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gbyfbrscd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/grfxpjbuc.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gufivegwv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gqlifkzvc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gbdzbaaxu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gkqkxunyb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/guaafnnwq.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdegtoywq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gsvpvkpdd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gvgqxuoem.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gorknoitl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gyagebdmf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwdvbpnea.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyzelkywb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/ggqqbdlvg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdaxpjamb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gpaqwlqkj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gsuhngyvm.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/grlkqsuxr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gcufunxrp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/goyouposx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gqrulklws.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzrmpewnh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gsnladcnz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gvlzythoj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/givoeoibj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gnokqnubx.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gtixjkkgq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gekryqdtd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gpiasoozz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/ghrhnqgcn.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gndxzztap.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gqlluuumm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gfcedbedk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gqtlqeqwa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/ghvoqbfca.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwdbrowyu.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gtxkzmmtk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqnfnblhu.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gdhxjvwcx.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/grenewohl.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gopsvvbqk.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gyuzyhoix.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gakdrlknj.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gtvhceanu.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gepzueazz.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gnuhjmpfz.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqjsqdapa.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gdaajqlip.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gpoozrlcr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/goggcrxpw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gdynellhd.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gteuwwvsi.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gxtovlfwj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gliovfzyo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gmvbcshqa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gdyfjbdac.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/geygdjrpc.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gsxrbhbqy.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gfawmfcnn.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gzxdlumhk.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gfofzczcd.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/ggrwulcek.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gjxqyuxps.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/goicogibe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gremdzqbc.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gypwffucc.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gatonjfwl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gncdkgoae.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggovsryss.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gqyqnbdew.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/grhsjvpjs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gflbdywds.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gohyldkxb.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gydjcgpao.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gixztlvta.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gsxxnnmng.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/goatrzlmm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gjvubsffa.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gysysrhsb.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gfizsglxb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gycevjvwu.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gvbszaaar.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gheohosdf.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/glkgzeumn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gqtakqxag.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gxeewkyhl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/grxgpjelh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gwctkrevp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gqnumqthe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gnntyccll.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/ggnbxmvbt.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gvjlomtvk.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gbwulstma.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gyjcjuqan.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gtfhxajkm.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gqbkuxwlc.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gxclnsnab.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gmgwecito.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gocoswpgm.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gtcyadsgt.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gwizhhpys.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gejillwwi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gfwtzglcn.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gvpiikaqz.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gcdeubcvd.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gwkhrpxie.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gypjxbqhj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gnuevmole.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gdtyfnuaq.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gtvekgtoc.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gecvlblkg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gccuuibvg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gybmuqwnn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gxwcrtagg.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gfawbahvh.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gpseovtpv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gfipwamjh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/ghsomlllu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gfatvrvfl.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gtnmcxltp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gzfztnfif.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gpwmukymk.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/grbbrwhsn.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/grzitoyib.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gniznqdzb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gpulazdmd.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gonfketol.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gdvnejffr.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gqhigcnam.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gmsxaqssb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gkqyycwhs.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gywalzhke.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gbyonjlnv.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gphagerzs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gpmsyqbkl.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gnmyeugos.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gegmipzuy.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gfjjtwvsf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/getnsbeur.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqupynhaj.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gfsllbice.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfpvszwlw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gmtnxodjr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ggknigrng.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gnmcudvxh.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/glesbhkzj.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gqhwcspit.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gpvbwfaoz.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gtxctjqvm.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/geqdibafi.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gbynamvvj.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gnvgwednm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gfknyczaa.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gmccxypyy.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/grvinihlr.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gwyjbuycf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gzuhjdgtm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/guggbjspm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gsoqmfjfq.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gqzudbuio.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gmznsuurp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gxamxanwg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gqkginjve.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gopuhgqwz.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gttbehbwl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gyjyhodni.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gxqqaguxa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gnkngsouw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/grqbqleol.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gtqolzpzz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/glxcjhcmt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gvyhlfcsl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/ghjojghal.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gpuyanzjq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/ghgouqucg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/ggmmwjekq.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/ggfjvyssv.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnaihqwdp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/govycfvxt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gqvasosum.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gfmeqcrqr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gftzrtkgi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gojwvkiro.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gmoeeztmq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmamreqzr.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gkhofhchw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gzfpfsqks.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gmjmqksej.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/glxaletwa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gzkqwgjdd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gwwiuxafi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/grvpmnnns.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/ghkfijymp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gyacvunnx.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gtwrzxuaj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/ggvnwenli.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gprowyzhf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gmgijxigj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/godbpdhvi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gchhluome.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gpcosuisi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/ggmysjqyt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gbxvrniie.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gzquigcvy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/geivgoqcp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gbulmzkyv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/glbadeaey.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gsqkrdnlu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/glsbqpjsu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gdmxfucjs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gbtyuniwh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/guirvdcbd.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gywfteftq.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gwcevdgzv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtqatemgz.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/guqxtxwiu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gxonajfvb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gsemnzbcw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gnokbicko.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gvgepdjkm.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gumrrbhwq.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gmesnclbc.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/ganlaocug.sHtML


<!-- 参考信息 -->