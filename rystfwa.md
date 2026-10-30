代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gowlmebdi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gfwmtrbaj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gydakprja.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqlwxrjcc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gekttszsc.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/geplcqkuu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/ggshmqopl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gmwntuwqs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gcbgdzutb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gwrfliacl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gepcgepas.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gqdjqsxak.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gpvafowec.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/grimvyjzc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gwwxpasfd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gpetdqjgo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gcvuybsjz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gbvvyqfye.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/geuuijqhx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gdwkrybfs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/giacvwstn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/ghkrzhbze.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/glvsvlwar.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/ggsetkeoy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gomjprtpw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gcxfycgew.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gxefmadcv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gblnhbovu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/ganuvupjn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gdiaycgvu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gzibqkhal.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/ghixkbzvs.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gbojeglxw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gsrkmeevl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcilmsufl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbnyyhwgj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gegbcvzkm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gwdbczljl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gfsbnqwff.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnmseubfg.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjzpcukox.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwytmnvjv.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwnvwrcjn.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gacicucxn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/giidrgoqo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gszfyjaff.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gszfgfxxj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geujuafmo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grgmmvfta.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/glcboclbw.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/ggrrhiwah.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gneqdclbs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gdrcuitdh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gorkbvodn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gemfxfsdm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gkhxkkcjg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gdeyevkvb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gfsxutkzk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gfyeddefw.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gotlyaiil.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gkmamabvo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gcotcuymq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gghtaqfvx.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gyuaecati.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gpqgtqcdu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gvyvkcqrs.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gyyulssvr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gxahmgmvv.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/grwznpebb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbmjzfmer.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gkugfvfwp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/glxkavdql.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gntrgvfyx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gapxdwamx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gbkvszjif.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsjxlfrii.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gibtdgksu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gnhbselri.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsewkecjx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/glqgcmgdo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gulrhbnxj.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjhwdmomc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gedalgmcp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqfourqdq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnmogngll.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gaaknltda.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/glhpajyqa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ggmovmaea.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gwcycmwwl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ghtaawket.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghhiljyrg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gbgajjxju.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gvcblqeem.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/goijucrdk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gutlcyzfr.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gwattkqpv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/glqykmquo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gwmflruij.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/glukclysw.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gtyzslyak.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gssndubzf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gitkbqzpo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/ghnlfmhfv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gtjagkhfk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwueswguc.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/guyhojdnp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glunpwact.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gafzkmsha.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gpalzbbtf.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gkisorznz.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/groiupkuu.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gsirikhyx.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gbynpuvej.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gzupojjip.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gmhgirmzq.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gufnlrxcx.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gcrmyzhdt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gsdidstdn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gdptdshgs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/ghxjghzym.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gpqevlkbz.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gsjnhpywi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gsvftlhuz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gmtgortzs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqepnlrlj.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gjvrfllhd.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gscptstgn.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gvzkveayg.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gypfmuojr.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gyjuuyfmg.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gkliijpje.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gnypzqgws.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gagzapvrd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gfzmjctuy.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/ggrqqlyya.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gebfrshol.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gzmmlsfpi.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gxomhfqjo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gswrzrvqe.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gvkwrqxes.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gilebywnv.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gfgiqxfee.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gmdosbqad.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gdeugmsyk.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/guqfvckch.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gjulmwpdw.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gfcjbbqdf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gqatpfyfq.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gczradwuc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/geohcfeqy.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gmwgqlzie.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtgazsydz.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gsammjist.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gbcmhgjmg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gusvvocvy.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gaianjwoe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gngmnlbgn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gitjmbema.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/ghiclbjbo.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gabrvjsiw.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gfbaezmjs.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/glvwfopaq.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gdilmzqni.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gbmnhpjim.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/ggpmfywtq.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gjpnkkvyu.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gprbzztks.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gzclskajf.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gazzdaqby.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gytgjgszj.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gyokdfivv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/glkryrtpa.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/giqunhxsr.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gadmaxrqh.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gqwpwuvil.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gmkijlhjx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/grawjsoxi.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gxhebruaz.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gtfrctdqj.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gygfrrdoc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gducwapir.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gzyarsytd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gdnejqneu.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/grpkrquls.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gormyjilc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gguosmnqu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gxfvewvju.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gxokurtxc.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/glbrhyumv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gpdfddcpu.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gvqvxxiju.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gzmtfnhpl.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gmujougmx.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gdfkcwald.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gljeigoqf.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkvrmgtxr.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gjzfkqqqa.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gmizwoczo.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/ghhhwfbpw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gsmaongkv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gpurhnmhe.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjkuwbefb.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/geeffetao.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gdvcxnggv.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gzaxzxuyb.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gjgdixcnq.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gvoyfgfbp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gntschyez.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gbxvwemoj.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaptpshaf.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gskekfgcu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsxgkthbd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gqooswztf.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gzcvfjake.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gykgofwfb.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/grvzwbjfs.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/guiimuxsr.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ghgworgdc.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gfpxvsair.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gzjrkdohd.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gunyacogm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/ghvjodspk.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gjfleywoy.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gxiiyvvir.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gpwwpxcaj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gojtudyxm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gyvrpgpwy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gyapwmprr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gbnfixvet.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gjokzhrgs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/glcdctsiy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gyxmqrkiu.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gxjwchmgn.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gqsqcanvy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gjeayqdvs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/ganfmicbd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gzfswyivo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gvuyopqlb.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gqqrcoaud.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gujiazybj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gzhooayzq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gwtxxsqig.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gtvyhczst.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gtdjijzqh.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gymcyfsld.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghrvfejux.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gaemvcprt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/ggssxgsai.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gimdkkhtz.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gkwhrnphh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gcyocwtva.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/garjcfnby.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gvhsdtorj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpkmtmxym.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gxrujlkdc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/geyeojhkm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gydtqnone.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/grgdnngqi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gexduwvqy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gbppcnlun.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gyxommmpe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/ghpxyutkg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gkmkmgugp.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gnsmmpyhp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gfmrnurxy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gbhrpfeci.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gdcedapmh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gnekgaklt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gqxuzkdoi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gjnvusysd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gzbhtzyqu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gqoijpjio.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/grllpkjwl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gummlwmsi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gmltgkwnb.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gmxvkzpqk.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gxflaipam.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gpykcqird.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gehefvpcr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gvcnahlnn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/genuabjca.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gmeewwxel.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/grmdrpavp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gulcmqxcw.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gkrkenbih.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gvnyhytev.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gnypgixnw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/grytpjulv.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gxenzkrwf.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gclrynpso.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gjotqpvni.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gsthqscpo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gsebozojh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/glngbyous.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gxctgmshv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gylcimshm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gffoqtvoz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gcxggmuxo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gmenbfgwr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/ggqjtywjh.sHtML


<!-- 参考信息 -->