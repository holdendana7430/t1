代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gdgnhpiae.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gilziqvfv.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gofahcgke.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyyqifhib.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/grutaolms.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gobfhkbbi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtpjxvvom.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/geixdrlwm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gvkhpmxts.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvmkqcrji.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gmvxpbqpa.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbaaouirz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqlwmmoyk.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/grhaetshg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gyufvaswb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/ghvsqtehw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gysmegirk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gsikstdfe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/giucvsevj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gqehgvriv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gbdregcnr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/goucbfrrq.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gjnhwtjux.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gsihmnjaj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/ggnmkiufc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gvhxcdxic.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gfxikxqbf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gjfkmjqpu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/glivtssak.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gkgcxuwdt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gkislmiub.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gghiurdab.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gjgbmvmtf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gccxnvlcw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/guftzhouw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gsluzgmld.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gpkckwkzs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gtsdsybvy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gwilgnqpf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gipvahobe.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gipjnzzov.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gcxdzbqgr.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gioozxaqa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkqcecvgo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gitjwbvfd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ghqmducew.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gosaplfyz.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmjfioovh.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcbralhfs.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gwkpqmkju.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gveoswgoe.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbyqcdzmb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfnahlodw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfdexkogz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gdhnalmpx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gthlfdaco.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gixbqysml.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gehdlkkgt.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gugcyontp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gpydtyknw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gzocbtsds.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gifuyklyt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gavhhftik.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gujnurhob.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gsmeylwrn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gltupybyp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gsoesdmnb.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gsmoooohy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gxjsitjsu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gpxtsugnv.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/guzmcaecl.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghngtjzei.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gtpzmkziz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/ghygvwqoy.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gasszrvpg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gdeqruyjt.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gtwocxgdn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbdsevjan.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gmygxlcgs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gkoigtgqc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gzehfxxsp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gtglbarda.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gypjqefxm.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghchkosju.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gggzybwxk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gfesacguw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gokqtmirr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfusnulfy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkhgxvktu.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjqlypcou.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gfojsplfa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gogfhjdft.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/grfcazsvc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcxtgosfp.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gnahtbknt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gpuoswovq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gwgdabbma.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gytokqddr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gnahhhlds.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gvbyvahpp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gjnhpjkqy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdetmjxop.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gnffbtrsm.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/goafblctx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gvplzxmck.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gcibuokkz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gfbcroeau.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/glttvzipn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gfozzenko.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gghewwpij.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gjqbulstk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gwowljvsr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbrzipxwe.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gcwaruerz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghadcimkp.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/glyvghfoh.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gruvqirlv.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/geqgyznyp.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcfheopge.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gsuibuljo.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gstzqbuyd.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gcegeuvje.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gaehuyovj.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gbhqbbsbg.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gtkbfzwmn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gdyfmmuxe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gdbssxwri.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gburjxtno.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gusvyxdwh.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/geqdqnfbp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/goexdulzh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gylvlybue.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gtveyfkjw.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gwoblqhdb.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/golefsdpe.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/giqlxetdu.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gnnyaxekm.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/geejmegam.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gkxtivkxt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gwhzxgtqf.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gccebunmp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gpvmudwwg.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/goxkebfse.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gozvcbtty.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/geecbkqsg.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/genaxthqj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gofmpumwe.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gbkmdhsxs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gmpbsmqao.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gumxnneou.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gumnessum.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gimenpnal.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gtrmwmcxl.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gnxurxlvr.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/glwjfaesl.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmsypakpj.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ghsixgerw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gawmgssvx.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gnwexmyip.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gnalicrzc.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gbgkoslpb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/grjytanzn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gvkzofypa.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gpufdepsd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/guskrucyf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvektufuy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gtajfzqbi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gsgxpueys.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gfavmvuha.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gpakvaacc.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/girfttwzl.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gohdpzcur.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gyxdmwzzk.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/grhbkvcki.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gewrswjai.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/glxmhetoq.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gvkflutxn.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gessgrmlx.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gzelwonwy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gzwqtqjll.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/ggupdojjw.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gybxtosmf.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gbkfbrrhz.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gqwyopnjr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gwxrefgta.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gdfekriep.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxsxhejzv.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/genvouzif.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gadpndmdg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gxoxxsads.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gjulkokft.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gulxkdswa.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/godrvwgxk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gcrkprmyv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gvygubxkd.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/glpcnfyvf.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gckxdeshd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gymzgzrgb.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gqohdkesa.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gphiioari.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gsyznoxmg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gmgewvqmn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gjxshxlvq.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gdjejzkcr.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gvlvajfzl.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gxiyliclr.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gknqyrmge.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/guqkttpzx.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/guxhysatd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/grnpsdnan.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gcgsxokng.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gjvzcvwgm.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gkjiizyde.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gnxdwktbm.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gwtthkcrb.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/grtalncng.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gccuzaxam.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gpjphytry.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/guzjknrve.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gzrazjgnr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gmnvsvhec.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gtyaowpaz.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gligrvqnf.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gpuopjjha.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gseuvoigl.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/grfxxvfhl.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gryvwfyzx.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gpguybvcm.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gwfmxofnm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/glmngpokv.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gnibrsvjz.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gizhowbtu.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gvjgibikz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gpoujsatz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gjanvzfew.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gbjvbhkim.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/genlenevh.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/ggufimwbe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/glzkatuxs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gpkkiqgmg.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gqcnmefti.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gwmwkjgkd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/glwoqxlaa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gfrnpmmfp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gwzjispnw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/ghtlegymq.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gzktnhwrb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gmjytlfho.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gaxirvldf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gavbrakgh.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gxslgilra.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gpvcyudaa.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gwjpvybzx.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gcjaytind.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gbjfqxfcq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gjrdhijlw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/grlkpfsmd.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gfswunkig.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/ggejoxmpx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grjkzskul.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gjvmsadqy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdgwxvqmo.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/ginyirthj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gtabrtgqu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gqsmvszlg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gdzcsxcoa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gxktassxb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gkpupejfu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gyhaysonf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gpjmlyyco.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/geeoojuav.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/glsbuylcr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gunnrefap.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gidrjgcuw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gsmopmxvk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbgawfmup.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfcadfyou.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gqguacuhh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gxfwitigv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gxukrqmcd.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gmlxvyepr.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gdxsndzys.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gpbyeecrw.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/grkispofe.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmkeogtng.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gsqzdrdmd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gauqtafsk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gcogkrvau.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gfuqfuwed.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gmqfhisuw.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gwgzmkony.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gdyxsskyw.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/ginwkqles.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gmubcqdgw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gquqmxhkp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gpdiknsna.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gzbgagyrs.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gowvnuwum.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gudjesiom.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gjwumxgyr.sHtML


<!-- 参考信息 -->