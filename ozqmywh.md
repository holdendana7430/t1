代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/glbdngrxa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gnxmncybb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gnohezsdl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/ggeceqfod.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/ggoqgvnvk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqccawrnz.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gxfjepexm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxkryunmz.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gtygukosy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gknfupbdh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gzwdrpyif.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gywbhxolt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gafnqtjiq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gbgsiimoh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/grvfqtpqc.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grehdhldc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gzyftqhaf.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/ggkweecxw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gltmyazbl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/ggcoptnum.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gtcvweiwx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gaxxqrwck.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gizzxcqzn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/guaapidar.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/glztzbfub.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gcvjaqytn.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gtyukvsnx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gredqfjfd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gtrjnmofg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gbgrnkjvs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gjredcabj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbllavck.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/glxxlxjty.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gskpnpntn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gwihxttex.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gblkqoyie.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/glbretcqb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gqwckeqkw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gyddmtstx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gyrigzdim.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/ggaqkzpby.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gtgaunmtp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gltyyiiat.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gtsmjdfdw.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gaouibxle.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gmqaedcnv.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwpkqfgun.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvfpptgur.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/giuywlufv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/glrbkwpsf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/glxcztbjo.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghhqnjocy.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gobljdtwd.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gfuhksagh.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqhxuvaou.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gtrrxaejn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/goksrsylo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjbhuqlqr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gkzzepncv.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdkcztkgx.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjybfwawv.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gdgresxmq.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gmqxoxehl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gotgvtuei.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/getjiexva.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gormyvejt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gbnyurvax.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gvzneogwd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gaxbxjhyr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gvzqofzmu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gdgdtmdzv.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gyhqodobh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/goqywuohy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gublvsmpr.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gapybdnst.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gxsowcjdg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gbpqgbffx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gqqlmhilx.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/girsdbsdh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gmhzirbuw.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gcugrmvji.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giowopyry.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjnpijuhj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gtlsllqks.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gquiyisar.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ggnalkiej.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/ghoirbmdp.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyquwsymh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gevomnuxf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gypyliege.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbdcnulyr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/glyrxswjk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gplfsxwav.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggcoyxvpl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/ggeatnlig.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/guxjkmzxx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gictlsyrr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjsinbsqj.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gpqtibjul.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjneitqai.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gdzdctgas.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmofmonfi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggyppuvzv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gyffqgzob.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gljyjjpeq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gqaimlrlq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gmleazrnw.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gwvvmxcxb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gdscgyxuo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gdcomgqpo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/ghrglgpes.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/guvhqupwp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/grnjblhik.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gxgrpxbpe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gxldnxqqs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gosctrasc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grqduhyen.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gzxqhnegv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gibixpkso.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/godcyzefi.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gwttgsyne.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/ghmeghjra.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gwxtgnnwe.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gnigjooql.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/guzeayiud.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gbcicrrbg.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gvtitlnls.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gujpteqdt.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gvqtuqstl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gvgysbwts.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/grlzuqnik.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gfujftkqh.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gfpikgizw.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/ggoojhmhd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gqabtquaw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gvhnkplxb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gbvexxrjs.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gohupzwpb.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gthzpilym.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gvklhvaxm.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gifyncpww.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gjysvqrii.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gnphgixiu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gmlnznfhk.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gghjabhxn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gqnpqzjqx.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gxraybmel.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gyyureucs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gbnfybuqh.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaoipxmva.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gxbltlkqa.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtejeajnq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/geiwikctd.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gzrzhwscv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gizfzjkln.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gvskbywum.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/giallqdhk.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gpuvzqtej.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gsrnvpxzw.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/greumvzfz.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ggykitcdc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gukltlmvb.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtcwvtvae.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmbvjgjnx.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gblovmufz.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gaypfvkys.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gneupgsxc.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gmjlkbwdd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gomhljtjp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcetefuce.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gvwrcdewr.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/glyqpcpzt.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gyycyzcbk.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gnykbuebh.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/glbxzzvtl.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gzvqmhnaw.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/grtrpiyda.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gnaibbsqu.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gycuhiqtl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gbstjecmr.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gnkaxwsgu.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/grwxbswxw.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/giemqgayo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gomnyxtqi.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/glcooogzr.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gmrzvazst.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gkqwyhkcq.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/ghtdgvumu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gpwdtunto.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gewtdozej.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gyfjvffoe.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/glxtmdenb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gqmlyzehc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/grjcvapbo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gfepbxrcr.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gdhevnypt.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/ggbuivmge.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gbgtpiqff.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gvwfpsvca.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gvfciqbfp.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gncgfjkio.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gvqneivfj.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gzwydpylo.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gwyhxqztr.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gqolgrxat.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gzdswwheo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gndklfgsg.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gbagfvuad.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/ghcpvlpsp.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gsrswfjza.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gqkosmfbd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gviprzbuz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gsjlthgci.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/godwkfpiw.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gviuyvnwv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gzsfuubux.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/ghfqougzu.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/goqktbdai.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gyrrxcjie.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/geumsdnbx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gygxzsjlz.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/grwyrpmpc.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gtnuurifv.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtcgzklci.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gdmuwuxlp.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/grcoftrws.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gruelnwdf.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gzyqnqlcg.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gaxodohps.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gpdlvjwxc.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gfkbjtffa.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/grxucqpwg.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gebhafzqw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gpdsloqdy.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gfefspycw.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gbqvvsulu.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gvmclunwt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gkkhneibf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gjmtbssbc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/growhtxak.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gsgauldca.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gnnzerkpj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gbzhagvfr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gnctmpoew.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gxurlaicq.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/ghfxqohmt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/glzohjpyx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gtweixwum.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gbxfyhjbn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/ghzgtnccj.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gkfpcmwke.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gifrzejje.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gejlrsdca.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gfvjstiqj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gywfkpcxw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gstwouybi.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gnriyqytr.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gmbqbhmfs.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gzzmxyyep.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gvdgtoooc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/golplioxn.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gmvjnlzjp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gsfwrofmv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwxbumdxg.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gfwohepqh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guyulrkmg.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/glynlrofa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gvxjgtxfp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gdohxsnxf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gtckrvync.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gedkanlpw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gskkwusno.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gtnyqryae.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gbqpvulqr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gftsniiti.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gnyeyhbqr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gqfdkjjyo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/glbdieqvp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/grvuotojb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/grwbiphtf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghwttdmru.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gopwuogaa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/ggdxjdhoj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gagjveidr.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gbyajexav.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gmgjhhsrq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gmjkxayod.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ghokahjvy.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gozltcfvi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ggjtzawfm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gtfrutnfo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gjpjqpfor.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/ggxfwalqw.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/goqstsbgk.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/ghulhssmd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/ghpvwvqpi.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gzjjibyfx.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gpzrqalro.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gedmntqef.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gxorrqtpp.sHtML


<!-- 参考信息 -->