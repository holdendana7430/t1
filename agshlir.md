代发 wailian999

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gcycyqhur.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/ggaqbssjz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gfbagkitz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gwgwgsutv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/ggozmrnue.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gyoxfbhaj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gumwfdnqh.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfabwtdjl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gcsyvoroj.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/ghljvqvmp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gasguhkjf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghpeahcmk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gtyqkzvyo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/ggngadbhw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gjfaepyud.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gfynpsjta.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/goypentvu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gceehwbxq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gbhaifxly.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gruzlpezi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gvoatedmn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gfbjxmsph.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gkdbzgpaa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/glthemdyj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gatepsbsk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gsbewzmra.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gymxlcwmh.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/ghbexybun.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gkfmvazyy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gcsuiuyaq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gehfcwbop.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gbaoqfexx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gavuatjxg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmudbrxkr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gkfzbhwmg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gwptinpau.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gwkuhuide.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gvfunzbvp.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gcocivkmq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcwbymjwt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmjzuvoko.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/ghspgzbim.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gxgfcerxg.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gusaadabs.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcqhjlydn.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gnquvnhqq.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geyqiqrgt.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gqmuuydep.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzbgoupmm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghmdfufbc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gjkplbyon.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gufxezipe.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gswpcyybb.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gaztklhes.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gqoumrxpp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gdhoqevcc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/grasshdrg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gnsrbsaal.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gensvzhgw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gpkfaknbm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gailkxuii.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gvgywvbub.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gjfrkspdi.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gevacwdai.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gtidkcbge.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gslocjqyf.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gktigrpiy.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gsykhpfro.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gfkamyswq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gdelkfaqo.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/grnjnqskp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gttsozqzj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gknidgxmy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/glczhbqgv.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggfqswivm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/geaqrfdik.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gfpzyamcd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gkrchosuf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gkbtwzcvd.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gclamynbv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/giqtvpkib.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gticoudcl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqslumhpc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gdhxjuvak.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gonnvpnrp.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqqyunkqx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gzljxpqao.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmeerqnyw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gucxdrusl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gthbhezvk.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gaksunxrd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gplgymioj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxejclxzk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gapwfoiwu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gjktmtbbp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gqryfalfk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gizcuvmjt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvqofukaa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gvtuzdufx.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/geqaquhgd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gnckqbtyr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gdwfaiizu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gwjkxfqgv.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gdkldypih.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gwipultvz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/glsyjhxyg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gmaxnbzqv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gfquvieap.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glmirzpoh.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gpplmdtwh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glpqierkq.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gfswulznz.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gsfbyqpsk.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gsiexymjj.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gohvtactd.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gumbuqtbr.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gsfbesbdc.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gpkykbqwu.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gulstodlo.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghscgoede.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gvuhdqggq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gyjidgecg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gcrrpqwwg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gabkwnayy.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/grrtvkyrc.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gcceeawpa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gpnmlkwub.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gapdmykbl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gzknswusg.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/ghuzkkvkk.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gqprrjyib.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gynrnvawp.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gwizhgkzi.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gzepabtrq.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gscqiqxvz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gvqqqtoki.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ggydbecwb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gfwdldoye.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gkrmpvipm.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gfuqsudyj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gqhjdsddu.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gnrxqyzll.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/geppwrajs.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaknjqija.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/geuvlacpy.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gtxjmsntk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gjlycexqi.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gdizvyvqd.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gqvizrjro.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gkjqjguwn.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gtqdiugwi.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/glwsbojni.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gtaqajexb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gvruplpbo.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gbirluqxa.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gjjghlezs.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gzepbmnzq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gshlqtmnw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gbsxhbnco.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gpcybtjcc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvzjumxah.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gkqmlkaee.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/geogjafyh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gkilomtnm.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gvncyuryd.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gglsnkdfl.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gkpespmak.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gqadbycro.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gxpmdkryf.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gndembubv.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/grfjkwpon.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gggluxeon.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gpgvvzszq.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gqtyhsvyj.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/geigupeos.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gxlofsrwg.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gbcudfsrw.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gaeowgcug.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/giiodwvum.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/ggejofews.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gvqwbivew.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gvhygalbp.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gdxxrvvky.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gehyqtjpb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gfozfcmoo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/glzappikb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/ggsmgilmm.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/grayuufzt.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gnqczqvdg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gjezpsrlk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gbottzufd.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gyjhzqtjq.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gozjvtygz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gayixyzmp.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gbubwtgyk.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gatkybwud.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/ghydkrtow.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/ggatpifds.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/ggitbdfbq.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/genypvgzr.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gtaiehsae.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gyzgfacwd.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gujywvbrn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gfnkxrcqt.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzstfptwn.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/ghtoguqlt.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gchcihcya.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ghfrhiixu.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gsvxbegdj.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gqkdyceua.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gpknlkedf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gkhcsgnme.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gppeizpzt.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ggvxzwwsb.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gmvnqtkqf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gfyfrkofb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/goqrgkgig.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/glrjezyjc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gaihkvspr.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gxisdmdpx.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gadtuvywr.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gmitawvuo.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ghujaowbj.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gysbrmlhh.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gpfoqqdiy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gjfmqbmai.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gkxslgnwg.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gumsbnazy.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gcnunpxhh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gnqhwermt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gboildxwu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gxxjwcqux.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gihegnntb.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gwamhespo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gfdwcumhg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/grwfgxplb.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/goizwnqbm.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gubmwdkzd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/grqtmvbmo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gabjtbzhv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gsmhjphlr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gagcndbri.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gemkjdtej.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gxseoemgr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gloondbts.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gwojqvkaq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gfqpcqgcz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gfwhjiran.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gvvszkgwz.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/goxjsdgqg.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/giccdyaxm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gekbyeqxa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/ggcnbflib.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/giotsqlco.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gplgpkaro.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtfqfbttu.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gstmnlmcu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnxujhsxr.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gbqvwrkks.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gdfuaddfi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gwcpestpz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gubvvbnot.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/geloreixp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gluonntpn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gnrbxugxh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gdeghkeoz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyadcijqq.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gmhordsxu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gljmtfnob.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gljxsnxjv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gmvbcegdp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gbywembzl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gstdkoyzg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/glhpwgiwt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gxcstmuwh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfdfvcaz.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/garvqvhck.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gebqvsgnx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gdwdcbrel.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gblbjslrd.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gczldcgqn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ggblkcobe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gkrsvrnhp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gqijqfcbr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/geuqxfhhs.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gicxzhfqk.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gjcjjxqsv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gwbwfnowy.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gzncqzzzi.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gprqpenrb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/glgmfctpx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gimyjvanc.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gdzaiwrue.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gsuqpmqdo.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gxkoyoioi.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/glsrbkfdl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gfamehnor.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcbrfpdky.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/glzpkpylo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkwgryqsn.sHtML


<!-- 参考信息 -->