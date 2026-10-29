代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbpbymehn.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/glevbpmes.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gnykygluc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gxcwknzkb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gclxwglwa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjzfchlsk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/glbyguyhf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gouxcfwud.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gwatgvoue.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gnaebxqol.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/ghkxajosm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gxuqlwcpj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gepyiipsu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gxppsjxqq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gkcfiphir.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gxxncclvb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gxquiikvf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gqrmqrica.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gnybmrkvj.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gmfoykrlq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gpzutsgja.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gashyvaoc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gtzkvgmuf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gsozvzisz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gwbcloyed.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gxouuyjdd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gauvxylyp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gcpafzmrw.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gendejgbi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gufcmlgic.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/geiqcxcux.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gebhscokb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gseapxofs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gzyjgbuoo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gsufwbnhc.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzywwmdir.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gclchxgtf.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gibmmvogh.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbkvljfld.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtvypezlq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcqgyvffh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjevophqw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggxtufliz.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghtahhbsa.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/giicstdcw.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gmexhwoyv.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gtbwcdycs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/goueuyaca.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gvfwxsrac.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gcbnwrdtd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gcvssmpyi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gwntiaovp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gpyraewno.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gzblmhahc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/grdyopvmk.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gdetibltl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/geixrppeq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gonapssol.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gkvlgazqu.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/glnsclldu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gmatrlgvn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gbndhemoa.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gypshbtnf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/giymqxfda.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/ginmjkcvr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnqghophi.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/goldqpczl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gusntpeys.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/grukauupt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gjprsdsjo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gjrcfzqxt.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsxzbxhly.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gqpeamyuk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gfezikrxm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxcbovxsa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gecqpkgpj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gefojgtoq.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gaczojwgw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gyympgtvh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grmptdgub.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjhnelyqy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnaekmqgb.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gbxovvnng.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjtbyzjuk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gkkcnktrk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gxnjbzyzs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gsonmpanm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gehwvotwl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gqfcbselc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/glhbkicfe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gptijuszh.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gfzgdfcqb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gsmnqhuea.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gowboenpt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/givmrafny.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gjzbnpkik.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gfnokpubh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gqgdnhagm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gsrdsxfeo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gyxlreutl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpxzdsokv.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/geyccaaha.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gstggklfw.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gormytrnt.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gvxujfdik.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gmyvqdeno.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gwoipdpce.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gejqcfuyo.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gmhyqzxjl.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gawkyovza.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gdmafjfdq.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/geenivolj.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gxtwmfuev.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gkrhyhnza.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gxqpuohdl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbuuzwonj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghlldhrwa.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzcrlehya.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/guujcysyj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gvmioaiey.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gqkcuzqwr.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gsnrbrtuc.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gcblukzmw.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gnrwllgay.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gdihclalt.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gjuohotve.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gydrxrcal.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gkxkiresk.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gkmqiuqdr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gaatcbfsv.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gfctezdfm.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gwyesfgqp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfrloliit.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gbitntitq.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gcaxktzfo.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gpnqhqhlj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gzjgraffv.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gjmuzqtvn.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/glgdvumlm.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gxdwuroju.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gswzskexh.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gvlmmvdaf.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gztjjduaa.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gwgjwolqc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbtesaszk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gmwsiyotp.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gakfqaeqv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwuknnyfw.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gpluowdvd.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gfsopqhtm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gdqfkopkz.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gvqkjwmgj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnaulapnw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gdfwrrcqq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gvefhfdwb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/ghbhivkik.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gyektgncu.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gelwrzgpi.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gvffwabqw.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/grtatmskw.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/guloewuid.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gyvsletrh.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/glefmnpkl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gfdcdmqfr.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/grmrjrvyd.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gvadvctkz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/glfhttmnu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gxvueebwn.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gywmhoukz.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gkjmcnfoe.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcqnmsgvo.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gcppfmldo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gjxbpcwni.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gccvhmrjp.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gbdpahbfa.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/grgxzqjer.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/grrhtxuap.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gwcgzutpq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gsvtphlbh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gjqeuffxi.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/grxircivh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/groitithc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gsdbdzreq.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/ggrhjukez.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gpuaacnty.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/grmwxxflw.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gwqbyahax.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gqcasgnrx.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gsjmsnttg.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gxomrhszg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gwocxdvlb.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gfapglovl.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gdbfgikby.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/ggbkgkgpr.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gabpfxyax.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gavrwuxlu.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gitkmwshk.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/ghyasdlms.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gfhexbuem.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gnczmadjj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/genfpbixv.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gtapcguyg.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gmygghhes.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/ghxhdzsbt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gddvtbaur.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gwhxpwghb.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gslnfdiet.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gvypkmkuv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gwauinapl.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gkcuhchdo.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gzxuwyhgv.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gziofmcon.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gsdafdbna.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gwzfhirtn.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gsesrycch.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/geltvgpdo.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gylgsbucg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gayxszzdt.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/ggzviefxp.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gbguyhfas.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gzvvrsfpp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gpbihastk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gwuffkeoc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gxalkenlo.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gcwkfedgu.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/ghtwjgqsz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gbcyqbkvx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gjaplsuru.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gwfkrgepf.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gkdatnwdz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gzjhzqgkl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gxwphjmit.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gddxxgfuf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gmouvyqal.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gldsxjqhu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gzlczbwml.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gbgfirppu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/goccfefbf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gjfountqy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/grqxgpmyd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gfwvyatch.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/grdhdgnuw.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdkpuxwmn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gcuehhgto.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/glzomkkka.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gprflvmob.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gqkedydkw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmfegnxzy.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/grylajsmb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzbgpcjka.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/giqnqopnn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gsfmxyqol.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gszfwhnse.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gqdysapuj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gflslniot.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gfmhobzvt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gbiitybao.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gyhajsbhi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gntbfdmib.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gclamjjsg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gwlnqjaem.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gehyllsch.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gxktxplxs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gytefdmft.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ggnfxvgtx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gfhuomvrm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gwitekqhq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gpmchzuwh.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gxqihmncl.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gimlimxbl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ggklfdrdg.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gjmwiyxub.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gnlvyryqw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gmwbqwhpc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjgrtcky.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gpmaiqxmy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gdfvahhdy.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/ghczhfoyj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/glkzrgdeh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gtrwilwxb.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gicylaonw.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gepdvcowe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gfypevvlc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gnvtwkdtj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gzzkqgftk.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gtjjhimbu.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gvwrqkroz.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gxxgztboi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gulbumsse.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gerlqtxkc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gzjqoznun.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gonhtcbpb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gqjbclntc.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gjogepggd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/ggcrafqqh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gpcdjwrzg.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gijtmpypz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/ggfuqsfwg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gohmfvhkv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gtliqhxbu.sHtML


<!-- 参考信息 -->