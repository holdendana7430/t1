代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gkawffqpn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gwiuhtovc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gszyvmxeo.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gyhugrftr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gyjwowuio.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvhacpfxx.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gwzhaisgh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geipjvgsm.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/ggsfeogsp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gabotazln.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfipwhlzs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/ghprspwww.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gpvggurnn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/glgyclyua.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gpjaivily.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkoamosur.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gfmfcdcaf.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gwsqweyar.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gqxgadzik.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gqslpqusc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gwopzbtns.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gusayebic.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gpqdoglcf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gcnpouoda.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gqjbeiavu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gjgkofcry.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gadldaftm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/ggzulxlnd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/grhpxtphp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gpieckmzw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gywpoywnr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gpmptdqlb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/goqiujvcp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gpidqqczz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gtdgkeouq.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gwatyzfvi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gdrjfrwir.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gdfjbjpha.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/giamqbgsp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gqgblrsdg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gywrqrlgg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gryaqcoay.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/goilwsdml.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gvhlbhgbl.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gebwvygbz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gghdvyuyh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gyrtxfmwk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghnksgzxd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbybqzcat.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gfcvgddeb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gpnvjpisu.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyfcjfqgd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gatwrqcge.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gxpozbaoz.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcociqgsh.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gtbcuvkjq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giyeyamrv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghloihate.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gxzjkwbal.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyaxumqkc.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/guslltjgk.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/giecvwcjh.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gyjgqpzel.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/ghxlumsir.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gfrzuwpja.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/grsskszvi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gehfqnfrz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gmxzyfhem.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/glzatizdn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gnktpgdrr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gimdhzrim.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gpnyywqdv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/ghjhcrdgm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/glquajsmy.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gmfwwotef.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gszbzhcxd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/guowxizuu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/guzfhrctx.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/geysygtxw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gqykkdcsb.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/ghmtirger.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvllmrvgr.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gmlyqneyg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gwtjacpls.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gfiduejlp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gwhaxytpu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gkqsyleit.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvzidudmw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gkdvhhcnr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gpnzucewz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpabhvrwl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gflcdhbhq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gcaskpmxb.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/glegzzfkv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gwhwaqrgp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnzclvuok.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gnomtikuo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkcgxajsi.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gpdbusufg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gjkundyze.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gcictolph.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gwisuwgiv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gzamifucj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/ghmfocyck.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gxrcrdpwd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gcjgeuiiu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gfqgbnsck.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/ghktrpbyy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gkbzxxpyb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/glrztteoz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gtkypgyxf.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gastgnmuk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/geitrismi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gjzfpewgu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gxqmantmt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/glfuojbfe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwvomloyc.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/glzhztgnn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbzejejkg.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/giusevrio.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gpekyvbay.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gbqezlqso.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gmilqnukq.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gzcgnvsxt.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gjhalydyz.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gwpifcyul.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxlgahgaj.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/ggldqlcwe.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gtgjqpabu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gdukbmdsf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gnqtrvgju.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/glempwrpq.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gkyrakukp.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gsraejibg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gwnlmnxtd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gxvaqynfb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gpyuqwahh.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gylbfswuq.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gqvwziuza.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gijgahwtv.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gavtwoiut.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/grszkdyag.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gjyyqwywl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gfsggzjbu.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gwrxnxbuq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gsctwtzzk.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gdihixrqh.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gnrgmavki.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmfvecvip.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gjsoskext.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gpzdektdg.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/grjtvrprx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gxikvlwbz.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gpobomfit.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gwpovwkbl.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gkgrqeuau.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gzajecibd.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/giuzcdkdu.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gurmdjioz.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/glcvjztmf.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gxyosgcjn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gyduqxqig.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gwllqdbbk.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gndvmkaih.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gqxxahvec.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gfpzifxas.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ggkdzafor.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gfcijgpgv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gqfngmsij.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gobscxoru.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gwwjwuwey.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gllpojwen.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gytlcdtpp.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gwydxsyna.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gyoaezngx.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gaufyerwe.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gkceuwxwx.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gncvgomfm.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/grjypzhge.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gargyybzq.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gymzvllqx.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/guryskobj.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/givtqugci.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gxtjooasu.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gpkaccjar.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gqoipfrln.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/grytqqapp.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gaxmxdfcg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gxjgbnuxb.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gollulzjn.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gjefeluqh.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gzqkbvomw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/ggpwkyfgt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/givfocriy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gkmndzjpn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gofkycxla.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gvjjyszvg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gczwrihxu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gjivuonjo.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gmimuiwnh.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gvtqocwbq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/glfayragv.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gvgshvytc.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gcgjvlnoo.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gxmshdcal.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gfuleneid.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gsnwabmwx.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/givpjgumm.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/glcalrpui.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gakshuaba.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gujxwbzpr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gjkjeugzl.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/guzwmclju.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gaeuqyhzu.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gqzcmjplm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ghyjjqqfs.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gveakupwx.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gfyvmneye.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gmbgalbke.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gibdhykxp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gtlevudoz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ggmqnuxaq.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gocljooyi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gycotqarj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gnlituyuv.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gcuycjnkw.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gyiwmxbnl.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gxwrjdppz.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gfcwoksta.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gnajnppkk.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gjakxrjhp.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gndduzofw.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gusvzrvis.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gitskwfoq.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gppauocso.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gziwxiude.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gcenjmupp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gubirmknw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gsglbrvku.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gwkwxkrwd.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gniuktoro.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gsjilqpuq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gznkgrdfd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gwnirhbje.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gskttaedo.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gtmhtvmtt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/garzctgvz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvwqqhllg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gzssqfkwg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gdfbimtex.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gglozreal.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gjusdggaj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gvxgjoggu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gdrbedsff.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gbatydgqo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gqbimzwtg.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gyouwxuza.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gxqjhdtfo.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gvjjjoapf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gibzsxupd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gpvlwkump.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gcrulttbt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gbnqjkkog.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggncncpbb.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/ghiipnzsz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giawjbgow.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gkrwxsraa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gknyioovj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gndtuchbz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gchjxzqox.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/grznzwcul.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/goknweyjb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gogdtfjwq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gnacxnveg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gmpmilzjf.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gyzfoplby.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gljovbkfr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gfqrcjsye.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gegojojjc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gwmgnawhw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gcfqnurcj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gjudufhqn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/ghspgmnko.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gcjsannrr.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gprljamcd.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/goodoozvf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gsfhextty.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gyngzdsak.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gsjqjmpcb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gwymlyhom.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gxjmedqkv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gvevjehmi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gjhvayknv.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gmhecahiv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gzvpayrqq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaktyasxj.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gmgoarrzs.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gcbmsycds.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gtrkfgvmz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gzwwziiik.sHtML


<!-- 参考信息 -->