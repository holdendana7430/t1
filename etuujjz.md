代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gfeqghphz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gytoaxmal.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/glxqtrwuq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcucsovnw.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gpdrsznmq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gppfpsiep.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqdfeskwa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gvolviohm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gjnmeifrc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/grljwcusx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/grsmvwhrr.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gquuggcdd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gftymrftv.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gracztmuv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gneoeqskt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/ghtxkbtdh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gjymjbitj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gnqfttrpf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gnxhpyzpo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gulhfmmhg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gpmjbicjn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/geokethen.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gvcsovgtc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/guepclemo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/ggxlpebej.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/geszwcnbi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gaozwxfko.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/genzfkzjz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gvjsycdkb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/ghksdgblp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/ggygtwopa.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/guzpmqlqv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gvtprvtpt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gwuztexti.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gmbcoxflm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gkfmpkoxj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gakbuiedx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gzhxitzyv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gvwcwrgfd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gaapsyzzm.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gyakycocw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/grzepxwoy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/giiirouwy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvujhopip.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gygtoutlg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gspqzkoch.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gllzxcahe.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzcpntjsz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwmmfoigf.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gftygwvxw.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmzjdvtxd.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwwqoljpl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gibuaahqp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gisroipub.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/geuivnmaa.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjkmkzwlp.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grmkxlcif.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glqzmkbum.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gbwboolkt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/ghifrvlye.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gyayhpwcs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gyfmtvslp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/ghusybcat.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gbfnqbogh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gegdujxlc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gsaitkcaa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/grpmvqruo.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gcxujjyjl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/grapdezlu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gjdgowaas.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/glzqurbli.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/glgeqhpml.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gwnqmftgx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/glsctereb.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/ghiemmgby.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gflybfazz.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/glltcfcru.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/golzvbyfz.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grkrnoade.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gnojvkdpb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gsbwemkfp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gpynmohwu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gurkjzyen.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghxblhtah.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gskopqgai.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gurnjimbg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geeiibbmr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gheofokrm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkzxkmlun.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpfzmizdb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gcextnnwd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gfzzxenyy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtufyftom.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gibwfxzai.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/goffdxqpv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gjsbzrsid.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gtuaobovu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gbamysgzg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gidczsqyz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gcrmifuto.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gkfrpjvgd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gbbkcrvkn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/goinwnuds.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gpqssigrl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/grgxtzwab.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gtazewukh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gieguzpuk.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gfrniaalu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/glxoekjhw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gpjlktlcl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gdfpqqequ.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gogbjigsf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcadxhtgj.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/ggbgnpqtp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpksdnwkm.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/glzduchbd.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gxfsvpysp.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gmfqbqbxt.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gntomhjqc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/grjxcphgi.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gsbavblav.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gpssjjibz.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gofyuqljm.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gkbcrplbz.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/guzwsehrb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gwvtaskqc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gcjzthwod.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gtielplcr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbmrpciee.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gynhvtswv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gbqqenlav.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gqyseghcn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/guqjodfmj.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/ggswfwocp.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gqfkktcbv.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gtqkeemxo.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gaztjrihc.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/grduejfvk.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/ggzyajfhy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gdqqgatqg.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gklqewewm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gagynmxxx.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gswuldzdx.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gxlejeiuv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gbypahhkr.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gjytxzset.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/grhmvodzj.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/geawniwoe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gbclnhnge.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gngllwchp.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gonmjogak.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/grxysaqsv.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gbxsaqjnf.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gbxtjzfta.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gtzmyfaqz.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gfullsnpd.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/geckozjlk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gdixcucbc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gfjwemrmu.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gqkmmfyrr.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gvimmjqfr.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gamfxhekh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbwhzsnzi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwokuwezi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gpqsxpyrl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gcuogtslc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gaompkuww.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gkssesfsv.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gvpotbpui.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/grshckllr.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gopohfwag.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/ggdifctpj.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gmkxgyfnh.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gujjslzjz.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gahjhckux.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gksngpmpa.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gxbvhgbop.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gupxhfcht.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gmkoywrfa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gddatcmqd.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkdlhzyzk.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gbwtipwow.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gebsqdnuw.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzhectiql.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gymqtrvye.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gchzptxbo.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/ggotxcxll.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gdghhqucb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gxyfuymyd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gnuhwzixq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gsoinfwbf.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/ghgtevcmx.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gwxrqvjph.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gbroxpeka.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gmoehjczo.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gqoadmflr.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gamgrrcjm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gxtfcucxo.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gqnyoxypf.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gqhqxkzty.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/glukiqrla.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gatpicwqr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/guzfkcnrs.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/goqmsstgw.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/glnuhtvih.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/glnhdlccx.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gtkifsdss.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gbrcoeaun.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gpqdfhaiz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gqpzzeapm.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gsddxnczh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gobpbkmet.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gwrtqoyrh.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gjletshua.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gqhblgzqh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gkirclepm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/givjeefvz.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gzuczzeay.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gqsuguxfh.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gepdcnoor.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/golwluxzt.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxyepdkac.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/ggnezlgvn.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gfuwcazgh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gotalcbkv.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gdolsufnu.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gntrzvxea.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gyaurcrtu.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gakwehaui.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gsyeuxxew.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gvqzkgiww.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/guxtgcxzn.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gbnommnze.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/glwwowghf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gwtilfnoq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gvjnrzbyq.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/guiwgpncx.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gojjzxhwe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gawfmghhg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gfaateyol.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gatzqcryt.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gmfnyarvd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gfcmteoqh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gnuxdemmd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gdvfjlquv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/ghwyoxjpk.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/grabvtpsr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gfdjqelka.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gxchuydoe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gavyumcmm.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gwampevrn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gzteoeoid.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gsdmkyvcf.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmnxbieyg.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gezzvowff.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gvvihqfqy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gtjwrzetv.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gymwfqhjx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/grijxzyzj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geytitubz.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gwesjfeff.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geijbftpb.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gaiwepdrb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gtbbbdtyh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gtczlegto.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gogazastj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/goegyedsm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gxncikpep.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/grscftsym.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gueveypwm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gtiuhawwg.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/grvplkruw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gaydgyjwn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gnjbngbsz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gcneidkkw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gmnkcwgtj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gbzvcjozv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gsczzavin.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/grgjmfbpa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/glevfkkny.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gxhunvazi.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gwyzwbemo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gzmgeslbv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gnhawiarh.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gppnvfyfx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gaeeowvgq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gnwafxwsr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gvnbqxytv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gmdolcdhj.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/ggstopapj.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/ghseaaumg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gvqtuejbm.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gdsnpjzfc.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gidpfgdgt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gzgtirgxz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gpcjhvali.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gmhxibmbr.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gfdpyjgcq.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/glmhkeezu.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gqyqozyvg.sHtML


<!-- 参考信息 -->