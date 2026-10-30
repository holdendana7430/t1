代发 wailian999

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/giwcgxfeu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/guzlfsoua.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gosobjmyx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gkgxzaihh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gebgwmtgc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gzuxnffjh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gcmsjusaq.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpyjcaurv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwjpgrrhf.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gejtjyjdx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gwjjlnxtp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gqrnkatqd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gqblomsag.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gjracarpg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gmwnaknbo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gpcnyfjux.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gjomubbwl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gnajoiigv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/grjfjhgov.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gmacekzkd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gocuvoszu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gbbbkjeqy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gbyjfdqtt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gvrgysznh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gpqdfvpfx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/ggraprhza.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gqjjefvak.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gwkofxhqr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/geovjvitq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/ggnboidns.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gubuaruwn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/ghezwgzau.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gzafwzwpg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gijriiguo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gkfjlfxoj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gbfzldyix.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gyqcihdcv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gbihrcjgb.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gopcxvkdf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfceycqka.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyalvcped.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gkxuskjkh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gbccsthjz.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdelewyig.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyilxunzy.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gbaohnges.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpuidihjb.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glluwlgqb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbtdnaarm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvkczumrh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/guyufhnzy.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyxnbwvdb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gryrdznuv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzfpwwjmp.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gqxlrfasf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gvalzblhh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/givmgzgqk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gvgkrplol.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gntwsuvkk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gfaltidoc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/getyvrhdk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gzeqjbdpw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/grfzeyqxy.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/glzoasvui.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gcodfofus.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gazggaaje.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gofbqzpwk.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gywwqnhvr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gjplbxike.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gofofxgia.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gxqrlezdd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gwqdnhnsh.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/ghlcnhsdf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvsfwmyhm.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmhjisazr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/grmmijmjy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gwbbpvglo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gjpzwtxtj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gdavjubkk.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsmircpsq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gxqjuajkp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/guetfuqqf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gubpwvmya.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gapodrfon.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnmqhbrpf.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gihauqtfz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gmnnoupsg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwgmgrtem.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzbcziqxg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grmfjhgjh.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/glpzkidsq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gbuativjj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gzshwwmcz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gdqdecdlr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gxxwayvri.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gvkdisxvw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gtdmaqchi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqoszhmen.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gxcsobwtu.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gvrmjssva.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gglxszqje.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gxauwjgbk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gdzkkonbh.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gapwtospx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gcgtacgfs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gdwupzsdy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/goxjfslkj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gufchnend.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfirmomve.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gmxzcqnvb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giuamwici.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gbfbvndjd.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gtpepjwvl.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gnlhavnjq.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gfybkjbtv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gojpzzrlg.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gavedbmre.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gdmelniek.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gpvwwmtka.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gjrlkuxbm.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gvtxzxeuk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gjoorzthv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/grntwjxdz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/grwhzurqj.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gpwmmpeai.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gfzviumno.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gwtsxsoxj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gkaodvjhs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gpjyhpyku.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gqznwuzvo.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/grykxaanq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gdyltmoyg.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/ggcmcgcoi.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/giigrplra.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/glioqxlrv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gmbfjmkhq.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gfapznvrl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gwsyqkamr.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gjaxwhpam.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gknntribi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gaqsaylfl.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gtnwxatml.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ghqdlmvcv.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gzmxdqopy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gednzphcv.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gswmylftx.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gdvhuukbj.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/glevawrbj.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gycsdtzjp.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/giknmlbqq.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gchddalit.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gaueelyhf.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gktolxdpe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gesxpgnji.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/ggmveeqde.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/goeiigbly.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gwcbrmiww.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gaoauokae.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqlvhvcgd.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gfyrqxtzs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsmqbvwgw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gjrqvfktl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gmntsndbq.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gkjbsxixq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gcbzrijwx.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gaclvbpkz.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gclxezqpe.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gjqnqqvzd.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gxaifaljb.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gdrsmeqxg.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gntuiomch.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gienoaltj.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gyixaudcq.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gujunwsoy.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/ggusebmfn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gvghizvse.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gytygjxbi.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gvsawquju.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/glllnxpaf.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gyyefblyv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gxnegcuui.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gxxzthvyj.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gjwoblufq.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gzlqnjkwn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gjqqztfyr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxguubvqc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gyidsfxxk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gytpjrwod.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gmzjnrjlp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/guaovpvov.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/giuaxttrh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gtfdsgvfl.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gvxrgpgdz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gzbqliuii.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gzvkvsnkb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/glazclfjw.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gdyjtrxkd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gftqrupnu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gjrikmblf.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gyenqboda.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/grykhvvzv.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gzywzumho.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gkotkrmeq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gtussdtse.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gypnoxhcl.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gscyuejsb.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gchamvssu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ggaduuvjs.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gmiykqlxi.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqpqovtzd.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gngtipeij.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gohkgvyqp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gpywspxlf.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gpvlkhjev.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gnoivxbbs.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gbiaasmmc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gnsasouqo.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gpqphobqt.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gapligthz.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gbhlbzcal.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gactcyjlu.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gzikhoojx.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gpjwbyeqc.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gyjoofphf.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gvhyxatvk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/ggztxxnbk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/ggwbpvqgv.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gxffkljei.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gcwdfonzv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gwhcnvurf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gkxiowbzi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gpdwjjruj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gciofohrc.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gwtdjojkn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gcbmvfwek.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/guozonwnq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gohyvwahe.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/grmtuylan.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gjhmxobop.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gxfdqyezp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gwjveozes.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gwyiwietj.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gjnazduwz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/glsspyxvx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gwpfuiijh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gynazxdse.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/girsjwfht.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gzkywzxsc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gewupoyos.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gdrzthjmf.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gnelosbos.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gyenggsrg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gyrmaipta.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gpblmcmrq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gzxglhbbd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyxssdzcn.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gyymwtwdm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gunruydeq.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gaikrbpks.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gmscfrkmk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gwhdpiumx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gekpayvcz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gpprsodqz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gzfazvils.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gsonwlvpi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/ggwrzutdv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gjjyoqttl.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gpzsftxth.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gfijxguip.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gsfogwsas.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gcmlyxkts.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gmuxytmjp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gcqywruun.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gwrrritlf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gemjhzmvh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gjzxummcy.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gamdazxsy.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gisdzmtum.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gmzlkqqyi.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gptonaooy.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/giddwhgcf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gqufwhwvl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/ggsjlwqqv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gaafoynpt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkrxlntlv.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gljvoonrh.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gmfmyajax.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/ghpttcnzr.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gqglmwbjn.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gqgvogvlc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gdsvmnzvb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gouarcfqe.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gmehgnnwj.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gyuxqmhdn.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gwsuqbgaz.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gkumeolqj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gffecddqi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gdovvatle.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcyomdjkg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gaczygpkt.sHtML


<!-- 参考信息 -->