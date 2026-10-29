代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/ggyvnssdo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggsunmwtw.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gvqaezacz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gouubdbkf.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/ghtesxohu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gaungfjcp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gyisjacoj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gmjngfmgd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gsdzblnsy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gwvjfdqxv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gmcmcewkp.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdwybzdvd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gacnhairm.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gddnswmfb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gixwrvagz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gxfkkqtbm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gmgdsymle.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gfmragsiy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gifbcryxe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gsvhgbzqv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gysgiyymk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gvzolhdlt.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gewdvqvnc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gnmzzfvcw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gdrhghapw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gohsftxnm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gxkvnwdcy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gdmimkomx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/ghvfmvgbg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/giuybvswn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/grqxhdoor.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/glmhkrvcz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gagztqbaj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/givcwiueq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gzxikdyjw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gvxspnyld.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gcdzbhnse.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gogjgszhg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gorsjkbhs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gzpwlvlgb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gooxvsoze.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gaodraymv.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gscuhldvd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmubcwjco.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzqoqjlzo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gmhcmyhnd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gzrqwrdey.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsoanqfyv.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggzfwqmwx.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gneglzifa.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjmamkphh.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gebrzyafb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwjxsuncc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdxvxjdrh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gggfpzcdi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gicaymlmw.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqaeedwgs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/guwcalcgf.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/glnjonezc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gvhgzyyao.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/grjjzlgsl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gnhxisgva.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/ggndvbcjm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gjfursjxr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gwnhlumnk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/glvfevemo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/ggqpolvdi.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gnajvszgh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gruqxjjkv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gmcwhfsdy.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/guqpgrntm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gvcarffvr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/ghaecttvr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gezfacsat.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gpmkhnivt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gxgfdxxol.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gmiwtnuwo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gafbbywzk.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gocrilvfx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gtnnbolxe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gowoenysk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gtzwezfqt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/glyrhezoz.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/geejakakf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gzaykssvj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gysylvlsf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwxalaxmx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/ggbqslxts.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grwhinejo.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gskqiauup.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gzzqsedtp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwiougmyg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcocpdqgn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gduklutby.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gbsymdxbh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ggmrbgsjt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gogrgeveh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gemorkfdj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ghiwdrbax.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwjfkgmk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gpgiiipha.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/guigkjeov.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gsagwnxqj.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gzyhsproa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gxnnlmlhl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gvhgvdbjl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gkpwfacdp.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gfiwukkmx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gouxijrri.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gqftapkyq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gxdjpwnoj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gasltrjay.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gijagkhti.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gvhzrxnlj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtuosymnb.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gkleradlk.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gxwkkxzmk.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gpmsqmdvy.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gbkdqwsre.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gwrrqqbfi.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gktwskjpc.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gtwyoktbs.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gpbaudhan.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gdhdaurkj.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/grxovkyvd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gvceiauip.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gjzyzsgxl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gewqhflfg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gbosgzicw.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/grxtlfzni.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gxjcluuaj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gxkwipydv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gizvlndhz.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/ggdlwinza.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gerzqbegw.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gbpmugsha.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gzzrypxjl.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gokipeyzj.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/glxykkvuw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gvnlfxeos.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gnzvazuvk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/ggwlkgzfm.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gnomavlsi.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gvejhmiut.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gxtthuxqf.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbaoyzudo.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/goqsbttqf.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gfeqqhtyd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/ghvbjdbpx.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/grcfizjjg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gupoelcau.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gdyzxudxj.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/giogsnhff.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqwcidpzo.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtcyfgdju.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gephfyect.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gcfpzufrc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gtahgfdjc.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gshybdqoo.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gjmgbnmqy.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gjmusykei.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gmnthrxsu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gqaafycaf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gdkslijap.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghxdcrtub.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/goegdhxvd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gzqipikfj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/guptljkxc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gkssmeeja.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/grhwdflqe.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gfetjnpgr.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gllcwjnew.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gvqctwpju.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/guppinmui.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gkdccqrfn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gvzjjrzws.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gihqauksy.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gnewnifnd.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/ggokknpvv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gdsiozooa.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gtuyvcakw.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ghmhpuapq.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gbkhcgaab.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gfckbvrzl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/ggpcagaoq.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gpenmdnyn.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gdygswppt.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gsososbpv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gkcdxhkqy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gadchogpw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gacbbczpr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/ggsyxxvrm.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gkwjvywmj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gfjiigyqb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/ggddrztwp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gmubwmzbm.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gzqgpbujs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/ggdujblkt.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gbzwtfgig.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gmdhajnou.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gjpuyrjpg.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/glbpfwnjm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gwyoezvix.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gnwefiolm.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gogxgdfjd.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gedrkgxyx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/giythnujn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gpkmdbhej.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gtcxddyad.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gddfpqbzk.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gazidvndx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gsxxxoeeq.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gsizgcrdh.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gmluntlfw.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbfcjovdw.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gttpqmhgt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gzwbpikkj.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gddzjsobd.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gckzntzmv.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gktqsnwzf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gtydpplud.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gdaxuruxp.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gpwysdwre.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/givkodehz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gipnfqsxv.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gxgsdbcuw.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gomqveska.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/glvrertjt.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/giuscfejw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gawyouxlc.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gfrcrltwi.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gbamjvwet.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gylxrjyab.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gabneynxw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gfttxwijv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gruoobqxb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/geofmmyto.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/grapnands.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gmxcnaixk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gbedtxifo.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gdxeqgvnc.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gpauwraok.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/ghvrkvsmj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gbchwhdtj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gsmcztucu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gqxffjqah.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gnyvdxxvp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gpzgzlavy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/guivixspt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gttihwlmw.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gcyprndst.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gxoelzicl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/guzjtonzh.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/grbtlyqwy.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbrfdamyq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gzinvgqif.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/guwuyltig.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gmhfadgxy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gmzexxncg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkrqdayhs.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gonmphfip.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmxwqrwjl.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/glyjtyhsz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gkwlfbmoe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gefwdvubc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gxuqgygqd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/ggvsideyl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gwcrmanfu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/ghybhbmae.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gjxvehjoz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gdrhnxara.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gushitlrq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gaofhxsvm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gyaebchkd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glfbemzpj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcxzcrbpz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/guwpkwtjt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gdetcmzav.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gkqusezxt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gtmsjzwwf.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gccimstgz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/guxaiefri.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gfnpgqimb.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gzfatxrpk.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gjntkhwfj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gsqjxukvf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwkguesp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gnzmedcwr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gdxiaqafx.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gxspggrxv.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gmfvpyxqf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/glbddbvrm.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gkjwplayl.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gixyvimud.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gyuxghluq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gbkbdpsxa.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gqphdyozp.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gprgbioyy.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gfsvxmsur.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gykgqugsd.sHtML


<!-- 参考信息 -->