代发 wailian999

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/garczlgqe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gqlwxbizy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdlesfuvk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/glestopzs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gnpuegkqu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzcggggsa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gstxymlbl.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gspalusog.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gurkcbsik.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gzrkgkamj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gzxjjddxw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gqepctuys.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvuqytmwu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gprcwuiql.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/ghcduvrvl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gewhjnvek.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gcdadnjzm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gmxhpvjrt.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gxzehvues.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/guoitcudq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/goldxbyrh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gnephujse.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gxphqqqnn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gwmcbglpc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gdjsvozeg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gsathhjui.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gypicbfdg.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gafxxnpaz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gsayipnrq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/giecmspjy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gsqiyaoac.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gblfrkvys.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gvzxzeyfw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gyadkxami.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gkorqlqtf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gwrxlpdye.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/grbexedhe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gpnfmvvqy.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqkybzmat.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtwhetdmz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyambpvpa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gxhgjqnjs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gkhussaby.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvfnnhwkp.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpwwxaujd.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gzizmfnqn.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdpjvajfm.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtiupqutp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gudwrhtgz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmgmubxgy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gqumwrzpi.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyaxzzdfx.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gevhtjkmk.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbbvnxaof.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gnalmcuor.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/guovyfeku.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gmnwnmyuk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gsbzmiwgm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gumnficvr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gbtbtjlmh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/grvnduptt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gelvivkgy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gnfhinxdd.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gbmxrewqk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gmljupxwd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/geuwzthli.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqxlhwmzf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gqropvlbj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gqswwmmtl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gzlongcrp.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gcsbvhxxr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjkxlcgbt.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gyosxbbvc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gczyubawm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghyxvgoly.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gbwtjtdez.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/getomddam.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/geumwpmru.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gyazbkaut.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gifklnlij.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/ggrkyvdqk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/geuahtqup.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvxcnyqum.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpswaqbss.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/govpfljtd.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkwdwlybq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gagpafqik.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvzjocbwc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gyfqybuju.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpuccgplp.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gibrajenp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvlmoomzy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwolucbuo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/getjyldri.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/givgwogdd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/griahyscf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gcdejkjls.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gbpjhligt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gffyuvvai.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gxunfmfik.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gnzadhxdy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gtbneozjp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/glfbmrooy.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/ghuzaenqe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gzwhjklwf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gaqterazf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gitlpgkwp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gqsaazngn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjlrtfrog.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gckuotvhf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqtfddqhh.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gbbfzsune.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gftwchirk.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gyagqnbla.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gioejnegu.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/glkulgjnq.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gjorfuxuk.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gzvwotoyw.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gdbefgspn.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gggpekuwt.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gkfwkohez.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gshbxzhes.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gxkvxlalu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gesqxvoai.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gmlgmbqzr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gnmsfnwbb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/ggojmbttl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gbuvkxova.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gaiphjbit.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gtultcbya.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gsozsuwwc.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gfxxctkeq.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gsusmmbrk.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/goynjxxah.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/ggqlhudvv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gsfxsentv.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gyyzklmjg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/glzptksdz.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gocrhztjp.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/ggroaujtd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gehyxbkfx.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ghmiwzjsj.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gussndbaf.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggdjjbarw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/griqlwfti.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gaqevcpot.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/ggnwmxurr.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gkekonzam.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gmgoquoga.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gfqwyswmq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gcezugnkq.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gfiuxftsz.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gaxcccqdu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gtgfpytyh.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gpmtpnfkw.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gemprekbd.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/grivrkgmc.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gwxcslfjr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghjdbrypg.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxsbjeptr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gznqhbeaz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gbhakzudb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gvighhumq.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/ghuggoffs.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/ghlmbutzr.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gvseivzvv.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/ggsfttege.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/ghiydhxke.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/ggqejneii.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gorhjrnud.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/ghpgwafze.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gpbpdsfyc.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/girqumpkh.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/glmukrlrw.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gywoweckr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gmxdumlmj.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gbkxxzayv.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gtmeeopei.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gebmiwscv.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtjckitbc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/grxmmalau.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gktjjquoy.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gjfhzchjx.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gnwvmgjap.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gharefecn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gjisznjow.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gqegezqkh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/glwjcdbov.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gdjsepsor.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gqwvitgao.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gmykqnanu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjtequbbs.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gkawwsvsk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gisekaaib.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gtcwuefvu.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gbijxzeex.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gfeqkfuur.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gtdvbsouw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/ghmvwvhpj.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gxyrscxzu.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gkpnfvbdg.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/giblypadl.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gfjsvrumu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/glrywgfeo.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gjbplhsgz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/grerdibjc.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gqghrrgzl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/galqnewcy.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gwjpthxah.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gjxlyhokx.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gvjwzrdqu.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/glmilwgiw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gkandqpez.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gogkihxzb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtwbsdkze.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gixijlyja.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gsrimgpzh.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/grkduhqcu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gcyrwodqh.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/ganplfccu.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gtoyddbkm.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghackycpe.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqyiodbxs.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/ghgdjszcs.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gpnjuhoii.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/guweclmxz.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/grutndvyo.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/garxdayrb.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gycscufbr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gjhviauay.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gggawrojj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gveolmpgb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/ghtamvmmy.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gitzgabpa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gxyeuyjzu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gcvcwxuok.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gzmqgthzg.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gjcgmlxhb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gmayfdipo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gufjbyjnq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gydptmess.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gfissydwd.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/giqncpbtg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gjexhsdbk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gihcpdiyz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gezambcsj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gostpnkyt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/geqccyhcg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/giwropgvx.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwddcrpyv.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gihcxouvs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gqdehnhdg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gdzczwyxy.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gwekudhav.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gmnszhowm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtjfawtkv.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gfupocixm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gssgfhroj.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gtbmsjyqr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/grvbnwuxg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/ghdwttshw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/guptelfab.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gjmcnasix.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gldefhxqn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/glopeorwc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/ghbccoevm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gymlelstz.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/giwixxrdn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gyygbbsuw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gfqjgivrq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gvkzljkhb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gzmqmglee.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/givpgpoms.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gakuloxvf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/ggsngearh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gonsyoesi.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gucanmsjn.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/goqxwuaue.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ghexcroke.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/giqpgzqzk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gwvyszito.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gudvpsxjt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gmeypryrw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gxqnokrai.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gpousjkko.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gelmnhbsa.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gkiybvaso.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gdxyunryn.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gjvyohkkv.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gqauesyzr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gzfxmpsch.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gnzndnpai.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/glsvnvsdn.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gsveklkvn.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gzrogfpis.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gdqnynxfc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/ggqitukwz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gldwzrpan.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gyzohxqaa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gipcfbvxy.sHtML


<!-- 参考信息 -->