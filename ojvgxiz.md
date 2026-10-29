代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gvkubuumu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/ghcvpzjpd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gvijrrpya.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gogspfvrw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gmpsrkbvi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnvugvvij.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/grrwwqoum.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gilamwvzb.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gmmxyjpnq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gdpnafvle.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqnrippgi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gbaoraght.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gdytrpgwa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gljjtbejv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gzqwcince.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/graputxll.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzfxelftp.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gegxaptdo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/grvxehdwr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gbyjusoxb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gvmwuwaef.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gjlcujtkj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gectewvdm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gtvdtouen.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/glnbphagr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gmkqedaim.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gpbsulwac.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gifrjhamj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/ghdqcvzpm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gqpnqoqar.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gjduqpnca.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gtfmrwfah.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/glghvleck.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gzjqsrvew.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gfnuajbcd.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/ggnhrdrvn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/glfpyvlig.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gbgpmkebc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gabtdzzfm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gtghlyylf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/ggjaoytzv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gyaqiywbd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gpjupdspw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gyifhslnd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gieavewzc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gsimqvaxh.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gsgytsdqa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwtcefcjv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/givnfhobt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gvyoqruuq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gthhguquw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvntfsqke.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/genexxtkc.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gkbznfcda.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghkaxanyf.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxsguavso.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gumuyyjzd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/grgtodqdu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gkayonzjr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glrvpwbvl.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gubvwlhvz.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsvdzwoxv.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gvkadaeim.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gnolhicpm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gyxqsdjfn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gzjybashh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/ghvqxdszb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gvnyaujmu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gufrglafa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/ggierzzvq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gtzdvtfgp.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gzawcnawe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gnjaymdxr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gvzqqwvyx.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/giuaqqrnx.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/ggzefokjj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/glopbjkrs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gloxwikdn.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gydqbellv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gfqyknakc.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gvpvwdvzn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxbqctqyt.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkxojganl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gxmhjpedn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ghlfupwjg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gsestojeo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gatmpumve.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtpylumgf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gipklmgkq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gmfhhssfe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ggsrszabp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gsvxcpgyd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gywmimpmw.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/godoihzow.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gcijuibgo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnjjndfyp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkzxvbpsl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gbwkjunge.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gfwwjncaw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gfqwwpvlt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/glgniienu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gipafznxh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/ggopoyyrb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gycegobsw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gyofcafoi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/grxqwsmgo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gbdzvjpgb.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gwgchumog.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/grambubzo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/giovranjw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gjbbiljbm.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gwtynfvud.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/geipenibz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/grrjhebqp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/ggwkoqwsz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gsedacair.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glefmujbn.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gaeefjkel.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkpolvdzr.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/ggxbkocqe.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gsrnhclpj.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gnwqvpdcw.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gxykzkrdv.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/goazukwue.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/grsqaqjlv.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gpqzlvaoe.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gcpqcmksp.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gvmfvsyfu.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gsqaqworw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gvrfzvcgd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/ghyoyvcda.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gjvbmhwrx.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gfsnbggoa.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gersabyxg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/ggmryvhed.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gzuqfcfvv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gnhznofqw.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gftuarcvl.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gcfgkfijk.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/geyfwobow.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gvimtqsop.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gzvpktmaf.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gxyxhgroy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gudypkbuu.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gyucxqvhp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gcxziimif.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gljnyxplq.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/glquoqqab.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gjcoznwan.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gmdfezflq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gtytawqju.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaupmmnvh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gcdclznpf.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/goivaidro.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gofnrmgay.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gyowjnvfz.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/ghkrvgrmr.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gektzoesg.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gtyjvcmon.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gltvwkztn.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gipdsbpay.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gsyrzujhc.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gljmazmhi.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/glhhhxzor.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gkectonkg.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gkjhdhlal.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjkkoibd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpyhkxrla.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gtcsfbjzn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gqceyfrxz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gpouufaxr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjhfldhkh.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gemivtjgs.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/guxrjqvul.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gzjfwxgmr.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gfngyvspc.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gnjuyityo.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gsazopssl.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gpktobwuw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gfvrzizku.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/glzheuzjg.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/ghbgaycmj.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gdrbvilds.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gsgkdsilg.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gizxkmvrl.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gphahywav.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gpxbylmxj.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/ggznrmpdr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gvpdrruef.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gjsoqokkk.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gkeefvlxc.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gdhfpxyig.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gvnbqxqjz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gmccfdshu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gcnhoqljf.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gozhohsfh.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gpqkciwrp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/glxawdbzg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbiaphnze.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gekzqezhm.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/grokiidic.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gqndbtjzr.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gzaugkunj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gltptgimo.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gxriiymhv.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gmhdszvkf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gcwmmhhue.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/guwwbbeez.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/ghsghbjji.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gekhzxiyw.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/ghtgprwgj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gnlfutobw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gozryznas.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/glyfxdamh.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gzekbxmks.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gmmbfqhpj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/glitxiawp.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gvyqtmjwh.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/govcyqudg.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/goudfjath.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gnrhiiirf.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/grzsxanjc.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gvzpdcttd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbhgferhd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/ghkpmpitw.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/ghghhuelk.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gslouyjue.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/grfixbkni.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gfnfelvpr.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gwrbhljlq.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gcfuclcyz.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gfhitoapn.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ghkzpkqfr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/govikrhzo.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gehduqpdw.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gvrtnygxw.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gvzxfrxhm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gbbaswxsc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/givbgefvd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gcxtiwnwm.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gzitkgydz.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gbvxdhwri.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/glhxejimz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gpyznjccj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gzgtlucrc.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/ggkpridyr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/ghqjhiobp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gmihcxjyn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gdtupisbk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gryhychxf.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gmpzidfnx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gaymtpthw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gfbmzkmqj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gworupwgc.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/ghubakztd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gcdqfpxdn.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gmcrbecdk.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtsrkvtrh.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gmzlftats.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/ghxyusonk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/geexoyfel.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/ggunswrwn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/grgplxrnw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzcmvblpx.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gezsexagy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkmogqtxv.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gxwqujzaz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/grrnhxkqx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gmnbrbwxp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gojaxvqew.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gfxxhdsld.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gjrvcaige.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/glekcwenx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gzvfyzqbw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/glpievkuh.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/grgnpwyxn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gvuqstasn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gqlwazmjm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpptclucj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gpqyqvknn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gqpuoinjh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gmplkmpzl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/grfdgjqjr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gehrbziay.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gchkoqogb.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gkyhebtfs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gtzfmariz.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gsawbtycx.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gstpapqkg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gmnvlytcm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/glgqgyxsw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gwsduhhaw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gnuyyvnxj.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gphkkzzyd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gmryohala.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gbpagvhxv.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gjpcvfyot.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtzicpgow.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gtacgqlkf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gmrphcxpi.sHtML


<!-- 参考信息 -->