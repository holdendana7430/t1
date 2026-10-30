代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnyhthakg.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/grznxdptm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gjmibobjo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gadnbjavi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbtxjhldj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gisvuknjn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gcvgpjckw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gtnbdywow.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/guqrsduld.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/glbrdqknn.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/grymvpclw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gsaixlxzh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/groeujvcn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gbhenrfpd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gdklxzgan.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gbcitxewj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gevjdmhny.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gsyujahtx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gfpohelbu.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gwbtikvqc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gongqrxxf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/galhokksy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpkjsvgtg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gqqyazyrg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/geppmdwgi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gcqkqfgxa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gxrlidrkp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gdehosefh.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gpfomvymx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gojmjihls.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvhewoqpc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyfectwhe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwhmquwwr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gajqtsdet.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gjvhvspig.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glzkwrjkv.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxzhbdwqg.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gxjzinhrw.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbtxdqarw.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ghbgaivec.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqyvbijtq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmftwtbok.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/glpljsmvh.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/glyyqirpj.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvptcamgd.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ggcbmufij.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gldhooych.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gtxrnvrce.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gfawkbrag.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/goghnjmtc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gzaqbzyih.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gvrolpyba.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/ghovjmide.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gelxlsvkd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gatzgswdz.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gdfztipip.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gapngajlk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gsrivfivs.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gqudganfa.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gyzxzgghj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gkoxdxdog.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gndansnva.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gxkxcakry.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gsgcspuim.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gkxymezhz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geebsodhw.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbgtuewpf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/glvhkzymn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/genlcernw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjpwmhaiu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gvzxgwejf.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkjjqidjn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gvjdqtcyo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gpnlhgbfi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghnuylrho.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/ggltwuznn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggvtiltzr.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbsfcfnqo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/geqnymrev.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gxliroeqc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjbftditz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gqgzvnjhz.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gaviurzgr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/goifdprue.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gqpkfwnba.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gssrkjjom.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gyvjvtkoa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gffxhjunw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gvgflbccu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gtadajjjh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/geuiviqhf.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gervqbxji.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gqpseiqej.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gcmogcxce.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gnvoevppx.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gnrbkegvw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gbkpdufty.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gzirbtake.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gzvzkfavr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gojwkhndk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grwphelbe.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gvptuyhfc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmyqaxqfn.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/guizyvlin.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/ghqgleihl.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gynkellpt.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gzosbpcot.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gahtrwhru.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gqfuvugid.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gpnikxpdr.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gkyrylrev.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gkaygugqs.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gjgrirful.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/ghrqrlpto.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/grahbkxjf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gnxgwdhby.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/ggggwzdcw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/geynqpozj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gkieiajtr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/girnpkfpt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gorobgdmh.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gmahovpeh.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gqrlfxfpq.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gxyaswzhk.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gonwejfgk.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gwqcjinkk.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gbqnfjdtl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gpggxkdiy.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gldkohpvd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gwssjfgdm.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gkllkaxbb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gusfmsjmd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/guzmldsgn.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ggrztcpnu.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gegcuzqdw.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/getqffgoy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/ghljnehvi.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/glbzdvgag.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gudofrema.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/glgdicrrh.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gzpoiiyfp.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gdktvafpe.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gcgmroooc.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/glnnzogfp.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/giybxwyer.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/goprnkmsx.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gvohomkcz.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gmkwlweua.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gokxfafyq.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gqfiyunxs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/guxthmnio.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gcpxvpjst.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/goufmjbnz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gdwxyiexs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/grlppqniu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gesdwzsok.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gzjwuwawf.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gcveoapnq.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gxtnpydzn.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/grejjzkam.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gqsvohmim.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gcubfllug.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/ghoyqtqlc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gcdqhxmne.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gmwqygaqz.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gulypumni.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gvdxkadau.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gwcbwijrx.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzedmmerk.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gnnudbzyd.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gjsmemvht.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gwuzmrvsr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gumlfuqcx.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gdafyfcan.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gxoxrmcpd.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gqbclzjyo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gqnypaqlb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gpoinlzwe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gapqxbgzb.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gywvbqblg.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gldaaawzv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gggmxtohu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/grclglbra.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gnmqlsiuh.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gbwidtshz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gldfvuojw.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gxxdbkkfj.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gohdygwuy.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gpbegfuku.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gnffnjbsy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/glbkaqlma.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gfwxrgpra.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gujefksvg.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gbyhvpzba.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gkvokazxs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gqlwqskmv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gtvwyuygh.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gyqnrahmx.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gevhottxk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gnwydixdk.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gagxoypzf.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gjfzddqhv.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/glbpweilo.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gzhoczrtq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkqnvxtfb.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ghiujoulb.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gelwfmhqz.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gprhcpxmb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gukpmluie.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gymiresto.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gdkbmcdor.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gwcmpsrme.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gjfbejafu.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/ghyrpdtfy.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gcsdmzpcu.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gxyftsrlr.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gcmignbus.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gmshhbolr.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gpyhciqhh.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/grttaxjer.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gbdbojlnf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gnokftilz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/ggtrxnngf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gpzspgodp.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gtzpafnis.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/grsvrhqqd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gklpnzxww.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gumborbxn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gflvjjbcb.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gfjwklfaw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/goapyjpma.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gdgytatap.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gdxoocptp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gzzuljvef.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gropqzhrf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/garbggbfo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gqyzekdbd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/ggehpztaa.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gmbhcxspg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/ggyuqpiuz.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gdryltxli.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gcskainhl.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gymrhfeuu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gqtcauwvv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gtshfocte.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gkhxmfyul.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gtrerwohf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkanifaxz.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gwpvtgwbv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfgihgpqp.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gifkcjbwf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/grlyojpih.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gwupkjwmn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gzvtlwsbl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gnvllrbgp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gqtzdubkr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gxpofkjva.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gslnzhbvz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/ggevfkbjo.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gkiwxhuzg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gczmppydg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gfmmufrdr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gyejuoydn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gzhkqvuvk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gddcdacwn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/guvzcwcwr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gltdshhgo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gnuugcbww.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gjclcfljd.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/glvybkpnp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gnqvovonf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gqofgqotq.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gxzmoqwim.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gnxpqkltz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gifidiujn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gdrftldab.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gzjzqkmte.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gwllhtfjh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gfzalstgx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gtdxdrqrb.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/guqqwqjus.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gjovakrlb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/ggcabtqdz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gfwiilxhd.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gxxtfbghe.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqaogjdtb.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gilowdxso.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/geaeekebl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gvfsjukwo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/geybphehm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvkqbglky.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gtenaoeer.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gzpamniki.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gomfoqjiu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gwpxxlrvs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gtscpvokm.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gcnawvlbw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gflaanuyu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gmmahawuy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gsfwpsphy.sHtML


<!-- 参考信息 -->