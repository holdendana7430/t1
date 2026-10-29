代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gtcavzfxl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqzxhnaxx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gpjrqncmm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwokpnvxm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcraestiy.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gfkbrlyce.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gtitbzdpj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gpfhxzkox.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gtantdnjn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gzzswucqk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gitxntbth.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gqxqzpdvz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gzsdbucmn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gznsojsdc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/ghyenhclg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gunbwzcwm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gxfoeonvu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gizhffsgl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gpgnzwycm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gimceyafy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/ghohioblm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/ghnthnfvf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gysfzftky.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gmdayslzb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gdyqcqpvq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/giaacmggq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gfmawjdlk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gnqnobcoc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gfvxreatq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gidrsrtkw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gcdmwmenv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/geekkrpwl.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gzsffxflr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gfyfcwhdz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/grtesdtcp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmvlokaen.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyazkwxtv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gopgsaxxm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gypyknozo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnkcrhjja.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbaojoxvb.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gzgybzmam.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmmxkdgcp.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gkiuwlsbw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guxdqdyrz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdwxnbuvl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gdyexruky.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggcoelffa.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gygyrrcip.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/guwapeuii.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gtqsmwgvv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gekqhbtwy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gwczlwtgl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gsnfuwhak.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gjrhxkvmo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gzumhaghv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gnxuingcc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gqgwzmvro.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gcedsgvbr.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gpmieewrx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gedvrdqdo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gqcrrwklx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gwulpelfl.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gucubkakj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gezfhpolw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gdxnljtha.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gwhtekbev.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gktsfntzg.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gkkywuzzk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gizqjitwh.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbprcnyry.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gbwvvpkvg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/glsuodewt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gdesqpmjp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/ghsgrxcej.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpengreat.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gjojusnyt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gdpwqtnml.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/glggdwraw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gjpdtxlmn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gitjettyj.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gefrgflyj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gibhxquxa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gsmbdptup.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gxbfevhee.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvusrlqmz.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gabrhbcag.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gejsesryo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gydxtrdug.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gsrobtmjc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gdkoxihch.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gbqxffnrj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/ghxptefju.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggujrnoxh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/goqaflvzo.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gbfzmxxso.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gpkbsrfrt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gkbmmrdec.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gifrekyuj.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gikkvuqbb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/grmsithsh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gjljffmbd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gfvnxpoqv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/grytmemaf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjiyankrj.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/giufmexdn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvfiagloc.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/ghoswdhmu.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gckznyjsb.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gvveqlway.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gozrqffis.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gfbbhimsm.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/glmzsycix.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gamtazohu.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gxrncisca.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gcnaxerja.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gqzbupumd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/grhgovkzy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gaoupkzkt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gmpucoonk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gxjubtrka.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gkrdyxbub.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gliiiskgg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gfsvzjtyj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gouzrylju.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gfhmzlrso.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gcugeefqd.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gcmlohzuu.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/grnuxzabc.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gphosnymc.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gjahjpjxx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gspjpmtjg.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/ghrpoeoxx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gzhybhdqs.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/guqjgibyt.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gavvycfrm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gsynhalep.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gbmwtkjum.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gijnkfgxl.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghcbkmfqb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gbdeymwhv.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gegtutwvq.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/govpfyxfj.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gteguemey.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gadbmxstc.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gtbhhyfgq.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/glgnyjrqt.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gbpfmzsoi.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gcqsjdiix.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gjnifbkau.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gknmxevlu.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gtlssitbh.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gvbldyidb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gxjsnugqc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqygtngnb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gptxcbqcn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gbkulkqol.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gftwmguup.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gbsjqssap.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/grnjavdvx.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gzrpetqdo.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gctbwyqzv.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gtonhdwzf.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gaytfrfde.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/ghwzexggi.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gbxvebrlj.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gtwfubpmh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gzrpjyexy.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gwlpxowqt.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gqgiprvux.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gnvnvhgea.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gmigzdzpp.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gmzkssfvf.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gftxhenbg.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gjikzznkj.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gvfxjlnjd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gjzmkhkxz.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gctubvqkv.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/ghiencqws.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gdttwuemb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gumqrluvq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gxczjoizu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gdpminjbi.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gbtcqgsfp.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gwpvbsknp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gcwyrqtln.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gsbrgaggh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/grmiizcxl.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gpsuiajal.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gmckjgoxy.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/guqptquid.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gakogapit.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gsfmurvmv.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gqwsengxm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gcolhnfep.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gmzdcexcl.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/geyvirbop.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/galhiytup.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gqjgivszk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ghiixavbp.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gjohgpcrv.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/ggxadeoys.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaxqmeaqi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/ggfqkveiy.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gvwibljrs.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gxxqsuzfs.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gygpdoryp.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gzgmtcqkk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/grjjupeab.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gytkfxjmh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/ggbmtjskf.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gkepiqzly.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gjgkmasxd.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gbdcechdz.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gmolsqlhi.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gldbpsfnu.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gzallusmd.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gmdejdkve.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzxflstbq.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gtnfxmqmn.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ggwcvulux.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/garjgimfb.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/giqwzihhe.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gimiqqcte.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/glzwprvnv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gnwjbseyp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gueeyyoxb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gxnwsxbwk.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gwtxiedwn.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gbmgjagpb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gccdtelpc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gcpquovar.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gyavjmuth.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gzvcmbcsp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfmfjpuws.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gpbczjtlu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gyyhhtbak.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gbpjawrwr.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/govqoaozj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkozimco.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gljkgketh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gafmwazvm.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gpvokllkz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gvjwdpkwb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gejqckoev.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gmafcpcku.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbnowgoet.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gklwsxnvv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gejwrqxiw.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gtsfujrvg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gfgrlyscg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmkcwdmrc.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gwhwsxqof.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbkoshprq.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gxoqfpvej.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/glawkbmas.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gxazekbwu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gnrgyvzyh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gszjtqdtr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gdtjuopau.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/glickiyft.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gqsoyxtyy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/ggrzvhwle.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gyhfqtzdp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gxjovzsdt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gedezacby.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gfszxlcbn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gguoyaisy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gumfgchgz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gmpxdxvtr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gbocybkcj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gnqjpwlvk.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gxjuzgomn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gtfkyzvgw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/goxjznskj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gcacehbje.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/girsnwxpl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gnirqslss.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/glivfkfwx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gzgsbghoq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gttohzjfc.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gvfmoxwid.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gyvfhlsct.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/guevahpqd.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gcqcmzzih.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gcsazgcex.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkzwpvmkn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gvqtlvkgl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/grxqvvrjz.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gsxvcryng.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gmxxflvgx.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gqfkqvrye.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gsvdwnqfx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gfsafhcel.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gqumqewfd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gruahaxqx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gkjklbcql.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gkvxelhfc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gvnrnkboy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gydourpcz.sHtML


<!-- 参考信息 -->