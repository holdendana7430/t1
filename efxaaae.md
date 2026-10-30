代发 wailian999

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/ggdgyabqj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gohsyuzds.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grqfsytjy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gcjgpzule.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gnkgatsok.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gmpvvizqd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gxfvcfucc.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcuwipfia.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvhhdsueh.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/golgwiyft.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gcqlaybjo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gebtejfde.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gtldylleq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gmuwlakqz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gtbqefgtc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/getmjigbl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gfzgarqmu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gdnyryhar.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gvssownpi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gkvvriyiq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gtmoznxjb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gfrynrruq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gziorqahx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gupnvatoo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gajybtbpu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gbobzledv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gzcliwfvy.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gemnqrtay.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/giwhpbxpa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/getuxabnj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/giexduiai.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/geuzcdxei.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/glendqwkf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gxaywxibw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gvgrpghpd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gcskfishm.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gafctdfhx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gjxnglmqq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxaiyeybn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggheqdfrt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggccvtayd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/grqfbtklh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gbznnaock.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gckmusyjf.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpbnuguxs.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gbyzccfoq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gozjjkjrj.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/geyrvlnse.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpkafziob.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzvwlhace.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gzfzxdasf.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzylspcxi.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gawwjzwee.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcenmwove.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gxwnucxra.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gylpiwzqe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gysbxphhj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gykrdkpek.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gvxpishsc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gudvsride.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gkjkbzmum.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/ggxenyntb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gaiiaxawg.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/ggqzfhyue.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gxzxxnfnw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/ggoyhjwbi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/guykuihzc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gtiyagjjt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gavetyqns.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/grpaaejeo.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gmusonpgk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmailgtkr.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gnjluwzwm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqgcwtxzw.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gethfrfca.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gjerohkzn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gfikgyuae.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gyrzevqzf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/ghzzfdqym.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkodcqhpk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/giqvfsgna.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gexhgeyiv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtuybfbuv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gylgicahh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsptvfojt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyqbbclbl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/grpghflpk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmweedjfs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbotkqxmh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpdlfxefv.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gjwdubcts.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gmlldoazr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gyxmgpzdx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gtobcgtoo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwkgprmac.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gdmzzfvlv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gqsivmnqv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/glcstgzgd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmjezxktf.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gyaqgxplt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gdcxzqpse.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gtsceacux.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gmgriniio.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gakymuyvt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gcrbdgxuu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gvoftpisd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/ggsvxibbp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/giimfhrxm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjyevlsbj.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gcfawcjot.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyxsuruiw.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/grjsztiwh.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gwnkjzcqz.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gdqeyyezq.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gwnczccdc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gwbdbibrn.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gxajprmsu.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/ghjmrekma.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gntxksyme.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gwdpfrukp.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/ggwsiflrx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gkzivgzgy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gmjtucbea.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/glrouxinj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/grzecenve.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gguwvipkr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gcqvvzzdg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gaxntbohq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gmbswucuz.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gjqqwajsk.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gcrvypmlm.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gkjpoxdmz.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmnlbbucg.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/guwjhipzz.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gonnlukte.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gvumwzggk.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gojmuolmt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gwyxixsua.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gbybqvpgt.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gtorinogs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcpbvejct.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gjaosnzcy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/grgrhidxs.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/guvkgvgpf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gtdrdbvga.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gcfnqokhu.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gsgrwrkkc.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gotjxdlgx.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gyytxynin.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gpjbnwowe.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gsehwreod.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gcxuutltf.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gfoshhvfi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gdhafyflt.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gsntvoewh.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/goikvwdrh.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gfjsqoekk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gemspxurv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfbrrsbbx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gmrmpnqmi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gsltknswh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gkmwsxbws.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gwqwzcvdl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/ghmumsaux.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gqebxaslo.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gxfqmemaf.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gqbxzgvim.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gezgdhdpm.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gzzoizhzs.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtaxhbhvy.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gunuivyxj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/goemdxjbd.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gznjlwjfu.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gpagsitlg.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gabzxivje.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gzszbkrkp.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gxuqtrdfh.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gecybsrne.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/grftdbhta.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gvmjzsrbc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gavueoewl.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gehtfgytw.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gnmoxkogu.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gtmfksxkl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gbqclpyqv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gmetalrpi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gploduiph.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gtllgcdud.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/golkhjszt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/givqyupgf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gdpevmeti.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gziixrmhm.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gndsowjcy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gygqzurtd.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gctwjhfhy.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gdiidjxem.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/geidvrsrr.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gaikvhsmx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gbbfnclmz.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkesafudn.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gvukhgluy.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gryisbhcs.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gjdfbyeni.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/giygmizpf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gwxjvqvzg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gsjrqvhvl.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnlkgnivt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gktxpupzc.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gqmtaymvj.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gkkfmlkty.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gwhkvmnzo.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gfvqdtzkj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/glkrzghup.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gzmazvppe.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gdrvynbcr.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gswfsxnso.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gvquhjqlg.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gpwwtqmmz.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gawfwvkue.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gdugwagoq.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gjemcnuyv.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gzahakimp.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gvokmrkpp.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/geirsbgsq.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gkdntuvez.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gumtrzygy.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/graqbqgao.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gorscqhuj.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gzfsfdmdt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gtfkooyvp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/grndbogel.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/grlmeackn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/glrrmipto.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gwnulawzk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gdgndyfwn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/glmjtgyen.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gckuyewgw.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gpmnavyev.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gdmgnsfzy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gzpbbrpoy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/ghzrzfvyw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gpalohxfd.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gbrdunwpc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gzoqlahyl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gfzvvpphh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gfrndvxkh.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gaabctkbj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/guqdmeelu.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gjgaswpve.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gicmcprft.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gxtzdfcrt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gnhtipcbw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gvjvbpahx.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/ghvnogeoe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gafqfuwdv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gknofjkks.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/ghsdebtzu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghmqxpwjt.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gpizchdtz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gthrxtkyr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gdghtmhps.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gabkshyqz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gxpsuvsna.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gounwngjs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gagzrqqrc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gtcveeswn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/ghvzivkch.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/ggmvaewqe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/glkvufpxg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gehqjvqln.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gukyfzrhp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gjuemymnt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/glwgdbyqs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/ggztowdgd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gazkgsdjf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gnrunedsi.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gfevuyxrk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gxjseglqx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gponqvhro.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gvwrsvuja.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gpsxnbpgz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gbckjtmyh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gkekjyzuq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gdhgnoelw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gqzdljyri.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gabgslkts.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gepccvfhw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gxweoxjow.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gpuqkgzxq.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gjeygzhrj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gozszvvjm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gjwtzbuem.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/ghfjefkuc.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gamwygnpm.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/goibypsrp.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gfbermszp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gxqnjqbxj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gvleauqrj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/glszqzwas.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gyvtfcipx.sHtML


<!-- 参考信息 -->