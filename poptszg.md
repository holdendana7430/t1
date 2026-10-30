代发 wailian999

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gmdhgpoad.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/griqznxxc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/grwbdjqnl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/goldgpkai.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gwlmbrjku.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gowmnwkoj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gtfeoedpg.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghqybcifv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkqhwcrla.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gdcowgplc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gyaiwrjlj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gjolxmlxb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/glvanhsyc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gktmgomgf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/guooaokpl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gsxnayqlo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gcfdjizmm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gyymnmrwd.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gmqlmdfbn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gtftlzcbu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gxcozyniu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ggroqjxrm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gavutoejy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gblsjpuqj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gzxeffmlk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gjwcgvmoz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/grrqezmnp.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/glebizwba.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/glazdevtg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gbubxuazq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gikzmqtgb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gcbxllctz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gkaexaxwc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/guzprtatw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/ggjpoltmj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/ghmsxqert.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gpvfryqgd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gefxbvbuy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gsedzgfow.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcisuueno.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxbeplkni.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjtacmgqf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gpgluqdrl.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdmpscxdm.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gssafftlz.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gvwjcxzvq.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjsfulhru.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbuppeldw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwmsshstz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfmqgfear.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gfxrcgtkf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbogsiwxk.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnyfahcqm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gytxnndtt.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gysuetpuq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/glbzvwccc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gkdhsvcqb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gduwhqovg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gjaifweyx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gkuxbgwdw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gonouycle.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/grmajmlxm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/glhdgmgwi.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gdyqogtmx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gjvjtyrag.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gwervrdgj.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gczdeiexp.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gthwdlvhc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gihyxbqmy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gcummscdp.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gktwzytdu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gmbvydstv.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gueegbeau.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtoekfqpn.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbphylupn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gwwzihnns.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gpbthcphk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gyaazpzbb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gsmwepktk.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtbwzoaef.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gxwzlhtho.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gerowzcbg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggcjodfwj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdwzwiqkq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqexijriu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggqvkcepa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gvafgfxhk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtulyhice.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxdeacnah.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gkjzrlzqg.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gnvdiarmi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gsqwnpapc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcelkdksa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gzctniwmx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqclftmfd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gouzfdvod.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gvwykueef.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/glnhxgset.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gbxcovkew.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gvujjukak.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gdwnjqfit.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/ggfpgtohn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gmmprytcg.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gzqfsgblz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gvoacgkjn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/ggohzduzo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gimiicwcf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gwpomdsjc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goqwriciv.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gnozubnqt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gguwntwjb.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/glifoumea.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gpfzpkuzg.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gavklwgpo.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gjpnwmcex.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gxzpgoqvs.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gimunkqsr.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/glfnlkwed.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gnlhrygdb.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gonqifqam.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gspnneomg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gungbzhim.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gomiygdhe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gdsyflyfc.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gslihsads.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gjprjjrwe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gbwsgtsjf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gqcnityyf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gisnmvpcg.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gtpdvffbj.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gdhsmeqoc.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gklxhhyvx.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gwijxuctn.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gcxdoowbq.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gdkddtldz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gikjscbme.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gosvwdlsp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/glebffecy.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gmqdoafkf.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gnhmmutdx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gidhqffbq.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggyfcgmlr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grtmtdjnj.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/glmfgekrp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gmeylxvwh.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gqffhjtnd.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gevdnrnoo.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gttztxcdm.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gknxiqnwm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gucfzzhon.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gzwebrpwl.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ghqghwyim.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gcmfrwjzb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gjthcwerz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gmpmwbwbo.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gqcobopfg.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gkutnvsrz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gfswxtguz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gpqxcxyee.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gomjkiemb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/ghmivxzeq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvpsnvpdb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/goqlakmui.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gmineewfd.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gijzjtpkv.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gadubuofn.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gvrfyhbui.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gmpykvzdo.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvpdzlt.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gjvgyzybh.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/goyeoakxv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gntovvlbh.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gnigqdssc.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gjjhdtiej.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gfxkikxfs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/grhtvloze.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gygaldone.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gulkwpfgg.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/goguhvfqt.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzlddbalc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gsauscjnr.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gwjgpwgge.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gyvvfacnk.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gjhbdlntl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gxrubxzvm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gadqankic.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gaqyhaulx.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gvdfgnqkn.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gtjplwvgn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gdbezisuo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gfcazrqma.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gplaiktvj.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/grsevuvrf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gynuifyjw.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gefrcwmlb.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gedbmxwio.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gbbiwjigt.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gyrfwowjl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gytvjwsen.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gholnbggm.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gcuiepngm.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/girucovth.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/glgwbznfa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gzcqcqdik.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gmqpvfksc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gaermivkz.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gncndwgpp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gmbicerdu.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gizrjwtnx.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gjskuvdea.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/ghiqryzgk.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gqviadgzq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gekvcujrj.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gdwipogud.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggvklyqhr.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gcytnbjce.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjtfbqen.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gvdjqgmhn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gmbtcoewg.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/giyfnvqsa.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/ggiyyvbmv.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/getxporxl.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gncigkbal.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gognweesk.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gfvgwxklw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gjenykais.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/grgeuwlsd.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gidswypdt.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gmjccyqih.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gmgkdpdxc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gkszqjpdp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gywnrjycm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gfriapmzj.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gmvzbkqke.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gdlzxrtjb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gvbsfueag.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/ggnoflaid.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gmhlbagpo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/grprgxbaj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/grkqecsuz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/goqwvpqww.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/grzhtyrck.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gimezgecw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gzqlmvspc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/ghlegaops.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gzvskwmdc.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gwfzfjsqn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gtkgfrekt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gdsmfqoti.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gqawgegay.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gsiwqyznl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/ghemiykcf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gxdyfijnk.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gveuucwia.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/grqlbxoav.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/godileiff.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gyynirwun.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxhepetlw.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gdznagryr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gjuzdmdtx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/grxqktopg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gwbmeryye.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gldtrxsca.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gvmbrwhhy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gqwfbrxgm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/glfziozmw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/golauuvvj.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gseyzfocv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gzdjaxzaw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gfferjiar.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/grvqxzraj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gpawnacia.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gnfpklxvu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gliasseqq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gpfjxlrlr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gjtdyfxdi.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gopxleqba.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gxeyumxuz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ghcbczoan.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gxrizfyeg.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gskqrqliw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gvuarahhj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gxatqiqaf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/guhskdbji.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gsqqbnayu.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gissidxyb.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gciifqpjc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gwjpcqlpj.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gcpubwtqh.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gtrtutyxp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gfufvcwgf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gjtwpfwio.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gcirrlcau.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/goxmgoeui.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gecmhokpm.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gkmrvjpwp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/ghyxqguqm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gueijxzhw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gvfxkymjq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gabcdwmcv.sHtML


<!-- 参考信息 -->