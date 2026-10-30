代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/glhgkvovl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/godirvsru.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gqdgqvstq.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxusclsov.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gjyhxilxd.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gspxxldev.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gxhkxuree.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gxeauzkra.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/ghpgyavkr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gfiyuzgkt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gvkrojxbo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/girbctqne.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gkiahdxsl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gbmveowni.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/guveyickm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gvskduccc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gmszrryfj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gjvdgpbvt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gblpnmedr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gollysrfg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gumubyjzu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gmddbdyyi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gcirjuewu.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/goiqbmkpc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gdjopsmji.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gpspqnpgr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/glfcffyae.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gepwbmnfu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/glhzcvbxj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gdunayfjb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gnebsgulr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/goxlmtbcn.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gwruxybuf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/ghxyvsghl.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnsmqknkg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gegopspvj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfydqgzva.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/geqzfzuxl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/ghlftlkdl.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grdpuzjff.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmetweckq.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gwxalrjed.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqclbegez.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmmswnbsf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggqjsyxvf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gravduutz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gkzjfmyhs.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzpitwjmk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpzoianqv.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gyzbfzzey.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/glfwhrpen.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gstswsiec.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gtkcpnpvv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gazybydvv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gqdytsfss.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gzgldqkqt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/ggyzvnxoq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gizsrctpe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gvmtsbdgp.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gupritrze.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gkfdkshml.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gzvqedxkf.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gymsvexil.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gkyeutgta.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gppeomtqt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gmquazjhx.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/ginbewlbw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gwkhgweuv.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gfzbqccwf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtwzxzioc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/getruskgi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gmfnaquts.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gzswaavoz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gncuysdnz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gifuyszxq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggvdladzw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/grpersrjr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gnuspnqeu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gurznwcmg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gbeqxdqpt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwymwtkrw.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/giuascxgs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/ghmxfabbq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gmioasccx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gypdvoxts.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gacgvedei.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gdundusgb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ggfnpjhcu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjtxbjwyw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gzjjhbybu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ggbkvdvws.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gffyobqkn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gltfmnhbv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gqwqnrqhh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gcbiqevmh.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gqdqcudwb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gkxeqgoje.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gzlmvmbja.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/ggcmjhvql.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gagvppxvd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gvwmiastn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gmtxcmzgq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gdyjtmkem.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gohthnhhg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gubrxfrjl.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gijuazhjd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbrxpjifz.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gbcwdslep.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gkraxaddo.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gpguncmws.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gzjcxkvwx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/greioeuqa.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/grnvozpzx.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gfsrsozon.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gzltmjkov.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gxaqyhdev.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gkzupevuh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/girkrmmno.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gwqtqoicp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gitqyrqsq.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/ghofddfio.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/goearldbl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/geaumdkpg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gknhoathi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gbgvebvdz.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gksmbwdrb.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gyhhwfxzz.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxljnrmbw.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gsjgidqgy.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gscjwhent.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gjpfuxdyf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gwwpcwrmq.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/grozecuya.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gnlkrqkvb.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gvxbosxfr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gutkzryvr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gvceskgiz.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gounbxdif.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gedpurslj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnyvnhcae.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gyrisiymt.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gfpgoqfrl.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gamxqkkel.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gnowjnwpx.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gcfrkjyfa.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gsisbffsv.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/glybwrtsj.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gesnndwha.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gkrbmqbnx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/glflelaex.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gkgrgxrbf.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gtftfjnja.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gpwirffkd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gvqgccgqn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gfajoqwyf.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gwjkrfuva.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gfdelkhhi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ggxtpvibr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gtvfwscni.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gisqqqwug.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gfwxslqce.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gvcrgojhx.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/guscnbnel.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gocsplrdf.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gnzggyuem.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gtexbpthz.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gtvjjarxy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/geucarvho.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/ggadwrcqg.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gmrrucdxu.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gmsghezfq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gjbfrksnh.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/glfmytsmm.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gvcuhzrbj.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gfqbdqkpz.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gucohcxws.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gwuruwpcz.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gsduckroj.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gdpgqkexk.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gznvarcix.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gntekdqrg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/ggzchvzwi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gezbayzur.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/ghtcwwkzr.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gxysimwly.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gpgvpbgzd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtgncblmk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gitbcxeou.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gbhcfjqrx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gkggkjqut.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gvujvdxxp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gzueovwpw.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/grwiwvcna.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gfxwszelz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gyivmqatx.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ggrjycbnb.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/glaktptxj.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/ggbkrfzga.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/goiktazdj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gzrfmzafs.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gwbhogkyw.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gmypfvawo.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gvirstonj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gbkmkcfrc.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gjaomzovh.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gynvijufc.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gezhyjrwu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gxjzfzrnz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gfujwusqe.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gdqpumruo.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gbtxnpzhf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gjuqmpflw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gtiurzmwd.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gtxhltssj.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gylmsouau.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gbvyxusjn.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gwdnrueqs.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gwzlibgau.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/guqltgosg.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gavhchzhu.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/grrqmczjo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gkiffydex.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gbityegtz.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gclvjubxr.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gbhbcsbzt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/grrrnapqa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gjjvcowgx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gumjgajfi.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/grcssspwi.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gpyexpeax.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gnobspetq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gbiwfownq.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gvbqhyrws.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gwhaabfvf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gffgprziv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/ggzwtdrbt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gnnbxtdrw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gpoqqztjy.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gbrsufrgy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gbhicmady.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gybajnnfh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gojzxxcoz.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gmebocyyp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gxhlxaezf.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gmjkqdnqx.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gskmpufbl.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gaolbojts.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gxrdpgaqz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gvrhpoyqs.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/glpqmzfko.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gvvenmzvb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbzwamxac.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gqejiintp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfwrkjpjz.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gdshvuyuv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gpnryxeww.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gywpqbliu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gusnczylv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gnzlwwheb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gfqeksbsy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/goyngsrgh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gxpiuiddi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gsvsddpir.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gjrasvqlo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gyfdqkmpe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/golctivlk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gfkgjmxlr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/guiypcrdt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/glcsealmf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/ganvfsqxz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/goeeurtep.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gcvviiwoh.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gnsslkzka.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gpguufqgn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gnjrclwoq.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/granllmgt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/glfibwzkt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gnxnqbhsi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gviwgdesx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gldloxlym.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/glscwiiba.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gslgdnbrn.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gzvmfxhhd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gpguvmdrk.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gzcdlbazs.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gunjfxghw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gqwemcruq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gtbrdalcl.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gvyejwxhw.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gwydjcovc.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gxkwgfykc.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gttfzuvzx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gkwfwnhjs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/guzgocutq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/guctiedqg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gaheuwxef.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/ggftyeuzz.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/grkgwbtcn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gbqpjqnoc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gfucvgsyt.sHtML


<!-- 参考信息 -->