代发 wailian999

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/guxzooiyq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gzvquprlg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/guhjgfhdy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gxcngnwxv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/grayiiwis.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gopwzeffn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gjclytfko.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gmicitaqq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gclnfczza.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggsmotkbq.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/getljscjp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtqkrqonj.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gllxiiibk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/ggualtnzm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gevbyhoak.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gkwsiscmd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gtgtizwgy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gmthtcxje.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gaxhhzdii.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcriknyuo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkwifmnbc.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/geniwthck.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gjcprmith.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gzneacqgm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/giauiwfcf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gwyxmrlxs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/geplfxjzt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gdgphhisl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gvfjwbulq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gygdqaisl.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gqeggzwfx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gutiqlvkb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gcxjfcpku.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/ghocuydrd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gyituekmj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gzbivomzo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gimzzfwib.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gvsjjvdzx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gozsatimq.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/ggjlqhkeb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gxdlhwdwh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gmxvzidma.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gljelhnli.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ghvwniuzm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gixgaqmis.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gigjuvpns.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gporodrgx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gvmfeyvdz.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gjmffdnvb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gdnaopjiw.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gwzwiklhf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvhkiyols.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzfzmrfgx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gwnggjthq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gkaoislkk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glbxzbrpf.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gulfyviio.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/ghfxqhoae.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gotsqlxnv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grsclsxmz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gudxlbtft.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grrudsmbc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/grjbsjbnb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gunvyajog.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbxjgiihf.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwiylauci.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gprrivupn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gejvmyqxh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gaoisnsyy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/glvzilfvg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gpquxoycl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/genbihppr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gymtgbtiy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/ghwhonyrx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gdccfypyx.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gfutfrfjh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gsonkhqwj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gzaofmxja.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gimolgikw.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gycrluiqe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gdoymtzxt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gkoaiqoze.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gjbuucgfc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gnfgdpkdr.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gntmodewa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjujeaatg.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzpsxkg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gqhiwuguk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/ghzrmrkye.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gvjgckbyr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gewruuits.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvwnfvpnr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gtnqmxsix.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gzvbrznfg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gqfnncutg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdaprpgwa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkgdlayca.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsasahfoh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gidxybboh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gwfroeydr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gaxssdaev.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gpzdquzoc.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gomwdbaxs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guggrrowm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gzhodwhqj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gwcjkagyu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gscpndbkg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gnigwpyqw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gasdiyygo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghohtllnm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gnahyfcml.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gqfqcpzdz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/grxjelord.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gzmmhziiy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gopysaihc.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gouavosvj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gazxhtbyb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gpsudtjig.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gjolyksnc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gkwncdwva.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfyluckgv.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/ggvpzuktj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzukpeinz.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gszaqobfs.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/guvzrngmp.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gqqogkbvb.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gogdhbvdm.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gpuzddinz.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gtdiakyea.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gxkapdqcz.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/grbrcxqnp.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gxvfoojrd.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gedugstll.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gaholivhh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gzbhywmje.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/goiatftls.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gticwqviz.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gfqlujehi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gtpoqxldr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/grezyuert.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gogctmalc.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gkdjzsolq.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gkxoiczpm.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/ghcqcdnsg.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gvzvcftdw.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gygjkaira.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/guysrvnnw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gjsxlkpvq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gtjlecgdf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gunfhfhlo.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gvedriawv.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gweydmegk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gtwqgzccj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gwhjrrhse.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggrhkyksc.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gcqqupfrp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gorgtcwzh.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gzzytxphs.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gveclmett.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gvkntqlif.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gjklmmftx.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gknarrhzl.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/glgroknby.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gchgqmqte.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gejaabbrv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gvtiwqpsj.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gdezdetjp.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gjfuazdwc.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/goyytssce.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gldqrzpkd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gvlggifdr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmdxcazwo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gvwvtheyd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdfpknrdu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gskuvyrxf.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gqojmmpnm.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gvonkcwxg.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gzcsrhkix.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/ggsucszxy.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gvmadqoun.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gmbgttitb.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gdbgqvfid.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtagnjgmy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/groigpzpq.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/godvpdtcg.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gvzpyvigj.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/goswscvrg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gmnbixrjw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gbmdyitvf.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gulemduhv.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/giodbgjnz.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/girltwlmu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gfnukssdk.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gqkqxkpan.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gnngqpvvx.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gfganetfu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gnyulkxkx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gfsagpgzy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gcndlzvqj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghemdwzic.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gqxjcmsxf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/grfohiezx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gfxkwljoe.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gquelpzms.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gkonranqd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gsfzsajwf.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gbpiozgul.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gpievdkgx.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gorracpvt.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/ghozcislp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gwhexsjae.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gyolnjyqb.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gtcbwhvya.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gfvwwlfcm.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gwhnmubed.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gngyrwick.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gucbdywzl.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/ggowpcrkw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/glybwfmdo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gvfdpasbk.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gubzkriar.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/grbwljlmi.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gzbvqcyzh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gkqtaufoh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ghgrtizsr.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gglrbjdjh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbdmxojnp.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gbxidxfln.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/ghubauvda.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gaymeumba.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/ghyfgdkwc.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gblblcaes.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gwnupzonv.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gojettqye.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gmaevdotp.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gqhqywzmb.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gpanlljzj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gpyhvfmqb.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gwydkkury.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gtdsvjlkl.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gpiowvhat.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gnsbbtqfg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/ghnmtbduw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/ggwphwgfv.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gwnjquutk.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gjyyufrrx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gwetnlmpz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gahxlgwzn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gqnqxwqgi.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/ggugpbmgh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/ggfgkluzf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gdjiehlwi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gdmxzaran.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gmmpcrsjs.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gxxawgvqw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gldnlsacu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gterwmdku.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gyzmlkolu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gawebwgxc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gsfpoadck.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gxdalkfsm.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gwbcezwsh.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gpwcgwxhi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gxmgjigup.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/grknwcrwu.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/geowtxrjx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gxcrmmpaq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geebdtysr.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gbzowsomu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnmsimfqg.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gosesvamf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gkaekjgii.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gzdptpvcp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gcfivawtu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gntosndtw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gzinpenou.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gcbwgsyit.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gimbjoebg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gnokiowrt.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gugnybwfu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/griwkzdlk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gtjraotcc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gtgtrammf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glwjuoaup.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gzdoluoza.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gbtvzfrzt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gzydyokau.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gugynebdu.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/ggdadsztc.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/girmjvguc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gemwidnzc.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggoflkigl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gfrflmslz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gdbvpyfte.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gbtvzgrmq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gfdbinord.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gtkdmhzdv.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gspmzejto.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gaguqcljl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gkppkiaio.sHtML


<!-- 参考信息 -->