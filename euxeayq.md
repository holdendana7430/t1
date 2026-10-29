代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/grkijcdwf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gjzffzwfy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gxhmqgwte.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzsmeiczf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gugonmash.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/guyiaards.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gfwhjwkwm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gejucezbv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gifseteoi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gbugbdrgc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/geebfelwx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/girtwvubx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/ggmirskas.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/geqxajyed.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/ggvwgotfj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/glalzotfj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gphbkvjig.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gukbfbdza.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/garkfmcho.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/grhplvmmy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gibnvebza.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gnvpnwrit.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gotlvduqf.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gxhutskyj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbwhzjhmp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gyxbbyifu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gygkjbfyu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gcntgzwyu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gpzjagqua.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gkdfxwtvl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gtymloqgp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gieapqfoj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gctfxlitk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gagunzjpk.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzzkkbguh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpnsodvan.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbciudgjk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gzjusszug.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gmcxifvny.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glekpcnol.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggfcyfsms.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gqgvizhtd.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gknflghey.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggnnacukr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gicqfiopl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gohwjatpa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/grhkxhekz.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gecfliyge.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gebhdtliq.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gnsdijdcz.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gstlldohq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gxunmztlv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/ggsedokoe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gwaudrfud.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gvphieeel.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gquhjlkfl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gbcvpwked.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gvnwrifum.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gmbisscrm.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/ghikpdsvk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gzmbzkmus.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gbjpaqqka.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gcmioqijl.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gppwetszy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/giopjbuco.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gwfwundgs.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gofsygkbp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gbmpyozzo.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gslvqomto.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggiqkvjlu.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxthrcval.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gzlhtftyx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gclrwzsoa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gandzycov.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gjijbmxwj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gobzrslfu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gtfynomxp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gnacflabq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gdcywzakk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnkzeywwp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjjdscesc.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gaxjnvabk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gvwkjmirl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtdusqmpc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/govazntas.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/guenzoavx.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gymzzeqmk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gwmcflcxz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmokdeygn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gkkifawpg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gephjnzif.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gxbpvdrhx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gkhcfqljz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gkuafcyvg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gnoscanba.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/goepgecrj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gejzxuaop.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/grupzpcrv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/grwdqeqwc.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/geqhyrlds.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gahzttjjp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/ggtrwwmhr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gzbpexaam.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gsnjikzrw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghybcrmei.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gheqdsdlt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjcvkpnfy.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gdvdwcmyb.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gzqwapetj.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gcqsjmzdd.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gayiqebfs.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gezjjucic.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gdretwfhg.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gthvuabhs.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gncclbsxt.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gyzniapdg.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/giigbcicx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/goxldgskn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/ghvhprxyd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/ggjgjnfxg.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gsfbfsyud.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gieandnte.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gduuzlpzx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gafstnmkh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gfkauezvx.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gaghhchnw.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gdvudvekt.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gyywxusuw.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gyqvspimv.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gjainqecc.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/grbftbbga.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gvvtmmfsk.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gjqmxgbpf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/glmlgbojk.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gfoiohgtn.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gpaacknhc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gxodqauuz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gzhzonknv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gilogpxlo.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/giqyiuhaj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gjhigerlc.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gzvixlslw.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/ggbvipcgc.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gdtzsinnz.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gtftuqhzz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/glwavmbih.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ghbyygdkl.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gogxkwuhq.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gnebbqaqz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/grfbzfvat.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gzhwpvvss.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/golumsbno.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gcpssujzq.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gngsfiqzu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/genfjaceu.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/galyasfvd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gogxavpey.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gwyblenlx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gdaemllfa.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/glmrvjjis.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gajfvcouj.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gbkmvvkvx.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gmqwbxtfn.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gxcbamkxo.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gsmqbybis.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gykdojlcm.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gewcgtqem.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gtwxhmrwx.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gztqjhauf.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gfgsbuijv.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gvslgqmub.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/getdgrxql.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/glhaixuqy.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gblsxbugp.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gweintjxi.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gjgmoqsoa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gccytnlom.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gqaqyiaob.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gyxilbzow.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gmdohhype.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gkwmcbxml.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gnqhbiqru.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gvevenhek.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghkoeqdgd.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/glilxscrm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/ggmifrfcb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gxiapyqzu.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gcrwzhmur.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gdkepcupx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/glenlhhzu.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gnjetdtvt.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gkfeswylj.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/grovvnrzv.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/giazqfhrx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gvlnazygk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/geodfvmim.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/glvdeszsg.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gwftjsoag.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gbpbsgfcj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gfyroqbig.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/glbfzxhfl.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gmmcektpx.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gbabxbcwi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gqjuexhae.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gedzhznij.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gyckcifet.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gywbajywp.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/grschxiho.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gjcpetnqt.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gdsgjkkkh.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gqccusufw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpvebvifm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gocbgujam.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gogxjipdi.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gmsqvwidl.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gblfqdpog.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/glzlksxwm.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gesgpfvfr.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/grsjlkzae.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gftzuezxs.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gtaqxrbvx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gudxihkzq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuhbksas.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gzuedsrps.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gtnshaqus.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gwmiusqkk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gkxbeohil.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/giebouzsu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gamwbvxse.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gldwbikme.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gyouzejuw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gxozsyxlg.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/goqztbcml.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gcrtzlxia.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gwadkncya.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gmhsfmcfp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gqpscainh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gfgmiatxd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gqrxfumal.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gvpqmjubu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gjontrcfd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/ghcdqnbmj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gkygmseyn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gagomnilj.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gtzhxgpuq.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gbfjrkxvu.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gefapnxxk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gcjzqbvfm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gnqmftbne.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gldqnrwjy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/guctkdpfr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvnzbjqdq.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gwaupandc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkzppypwz.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gzvzupmdd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gjmxjhahx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gfebowrex.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/garjcxhmx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gjgvtsgkb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gmdyxqhbb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gsboxfgiw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gkcveokjq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gfiqydwnr.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/glklugzxm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gzyvhotcp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdubxhdzf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gfwgaocwd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/giyhtnihf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gshpnngbv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gmtovdfvm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gbpiewjim.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gfrirguok.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gxxymlchu.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gomgeunzm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/ggycbhrjh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gxqxmkoba.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gxozoiixg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gnpqxmacz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gmqobeoht.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gmgncjrgl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gbesqbuot.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gjdaynath.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gxdonuntr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gqgyjsqsk.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gikhhqenz.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gmnenuwed.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gremxgdez.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gozistbfq.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gzhubstlu.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/ghpexudva.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gzteqbaza.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/ghyewwhjq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/ggjkwlbme.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/glidxgmsy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gmxhlygly.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/ghdzqdbbm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gaallknrk.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/ggxbwfaox.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gjmqrijcq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gmhyxbhua.sHtML


<!-- 参考信息 -->