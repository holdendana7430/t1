代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gerivsvtr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gzbobejna.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gusapkmgq.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkvdyqkty.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfhmogenw.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gqlkkhmty.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gknxrnbhh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gsuuadzxx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gheqfumcp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gftmbwwkv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gdastxnfr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gktlzbeeb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/ghrdjnmry.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gvbhosqie.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gfyvcdgkk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gvyrqrlia.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gsxaqznav.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gujxaeeff.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gtihmrjuq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gxswqkzbn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gbtlrsztf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gnmbqcfts.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gqvcvsyun.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gbpoinxaa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gghsdyozk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gsvqfhjir.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gftnfeyxr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ghuvxszlw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gdlabawyb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gxlvargvi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gbrewszvr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gvkqyjrar.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/ghdksldfl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gwmfrjnur.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdwscqsll.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gerrfvosf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gczdqhyce.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gznfbvylf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gucspqsyb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxnonfpas.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gugezawry.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gyijenrnh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmzqlxynm.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnztpqtll.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggwxogkqu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggoluhxyp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ggrbdqwip.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvhobnpcf.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzjrfyxwm.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gdzqxsynh.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gobkjtayi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/glyrucynf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gcwhixmfu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gehmwxuuh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gukwpghhw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gjxrbczem.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gxntnkobh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gixcuzxna.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gshclwdhx.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gozvtpkgp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/glfjvljvb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/glkkkcvev.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gdcoxtdoo.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gtmbuyuwu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/geteiasce.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gahgzoytp.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gfczyzvfw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gfhmlrvtj.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gcllhzkgi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzpmrvxxw.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbsiwgqhb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gvdnuawyx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gcsupntwk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ggkhxdcmi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gvmxkhhyp.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gopfqsltg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/grqnoegur.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gdgerrdpe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvuflnuot.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjeikqzzr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gakktmsui.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gejcqjvoo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gsqqxxphm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqngpyncj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gabkqhsjc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/grlansiqp.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gcovckxpq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gclxajvjs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gigejxqzw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gvnuuhzgy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjldhylfe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gdmzgntkz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gbltenhti.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gvgrhrhkf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gzaxavsra.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/glyepzrgb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gpulixigl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gtjsnikmv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gugdeqjbl.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gsxdlqaia.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gcmniypje.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gmyklnnhh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gotspserx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gcnzzmdgi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gluofloau.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gklhxseiu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfsxoapkd.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gnajspbma.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gsbvmlzhe.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gqvhclmgq.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gwugjeeep.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gwrragclg.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gaqxeminr.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gotwqoemf.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gukhefrcx.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gzmzakruh.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gplmsoltz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gzkhisbmr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxvzcokub.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gzmvbvaxz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gojtjnhdn.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gzabidnpf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gtghsbasp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gyjbakybu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gohmsgmbi.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gdluyvvvu.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gewmvidsz.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gaabrrsaz.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gjthexioo.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gwmumqdcb.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gqdbipmsb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/ggowxkdhn.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/getkiozys.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gevgdkudf.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gblkuerjt.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/grzpbhnzs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gzsdvulfm.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gxbxgevck.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/giqubqwnp.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gwfcpuvkf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gfsdtsfxp.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gyullsmfz.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gmhctpxuc.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/ghddipxqd.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gkoyxljze.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpohsojuw.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gostqocnp.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gwyjkfbot.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gbwqcmpsp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/guoegceuh.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gsxuvybxm.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwkhhjx.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gicirdxaf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gpnelwejd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gdirhqebo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gyvtaaxqg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ggdvyuyrw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gznxjlfmn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gsdywigrl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gokxtooqp.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gejegeamn.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gihfvffhe.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gueyfiews.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gpdzasnwp.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gbvjonwvx.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gfzhervfi.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gppljsdee.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/grwncqfir.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gtzjtnkgj.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gekxtosob.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gxefjpeqv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gusujetpy.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gayujqnsi.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gkcfvlolo.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gaiwueqtq.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/griapekky.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/ghwpybckj.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gusnxmaxi.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gdlrmttkv.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gologmwdk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gbxorftoh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gpvohwbyo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gnqxnrubk.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gaidctjli.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gykckrikz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gppqfchii.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gtfpaxyxk.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gwocyarsq.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gwmywgtcx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/ghecpzyvi.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtqwnypwp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gwlhgbhpk.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gnksicvui.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gtcvluagg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/geududgph.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gshvvijqk.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gqpnfkxld.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gjybjjwlu.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gbnsgpfwi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gwjpgyjyf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/geswbpnmm.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gpcqgpfci.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/ghjjurcej.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gzqmokcsr.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gnafzvzil.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gcokmmlkn.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gkvelhgxp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gblfqshrj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gigdsyzxg.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gwzktuciu.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gxhcswohi.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gguuzdwzo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/geojxdgsb.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gjpvrunty.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gcwriqhno.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gjgwrhlyg.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrmxbafl.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gqogwwclb.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gxgcaxkfw.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/ggtjkaedx.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gtzummtxw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/geeprbdaw.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/giynjtgmc.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/guzpxcnme.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gedvykvaq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/getjxjjvd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gecnynbmd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gmxlhcetn.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/glrbezypp.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gcpxcdkwm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gerodhgqq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gxyzjijni.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gzdaecqjl.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gwlvztsai.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gsgbktxjd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gudrfsxnw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gfocfctru.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gqifuujqd.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gvoejflqn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gqeunzaxx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gftnkbtoy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gxpdywfos.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/glbopadoj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gcqzctutq.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gaaalcpqa.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gevcnhsoq.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gdbdttcmq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/groevybof.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gkvbacaba.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gkgfsnswj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gsjrvklcs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gknrlafxp.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/ggmqoqlpl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gliqskitx.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gauffkkoy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gdxpmjmwk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gagvfxeul.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxdviglk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gwdufnxzh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gmffalhwy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gywfqnymz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gryhfcxcd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gapvesksh.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/grmoxjdqw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gfwfwqmzh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gkupszixp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gfawnvxla.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gkjrwnyqg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gbozddubs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gmnhztouo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/goeiwcmfj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/galipzvox.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gexqtjamp.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/grrixdcfd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gwivexmwp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gnfifpkbh.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gpzkjgwin.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gcozqhyci.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gdndpmwsk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gxdekfjee.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gsfoxoipf.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gzqtqbynx.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gskemkohn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/goawkikci.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/guhvdgbld.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gfkfcqsyi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gcglspytn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gezklmoxv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gcfzofopt.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/grzfquysa.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gmnmrecwi.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gatgbdbmm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gjsbxbxpq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gitodqvvb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gceodwtpw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gvzcajtda.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gjfxnoioo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gmmohjpxb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gzpgqjhfc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gvhglqzex.sHtML


<!-- 参考信息 -->