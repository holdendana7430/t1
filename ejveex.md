代发 wailian999

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2tdirckbv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2yubchwku.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2vyksmcym.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2cpuzfyqs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2pgwovkmg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lhrsofbj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2savjhbtx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xuzdpxjo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tgxgmxcp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gfowpmmj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cumqpymt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2agimiala.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2kcghkumx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2bzlnysjy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tbprynhw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gcescilq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qvncegud.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mttsmgfe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cblribqi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mdpuykbq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jkzlupvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epjuyxua.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fctussdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myqogarh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlklorrw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2uftbajuj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ywbmheee.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2oypnzdxq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tefwtzkx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2spfxgpaw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zpjznasf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flnbgnzm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yfohogdy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxnbnvzf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2chwwmkph.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zfnwrnkt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2quisqdtt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gvyzrzwb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pqyantkp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wnayglgk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pcadcvyo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2lyhkcviu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rfhobkrs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yeyrfgew.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2umuasbnj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wlggoqff.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yixdpabx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dzpbicxj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bqvzxlav.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yehxaswm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gseowhzj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyjadlsx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nydqgvck.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ticekbht.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sjjvmiql.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ualvyfbt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wvxhesla.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jyddssau.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2outjdwad.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2hjceubvh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bgyluyhx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2engwmmtk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ufocvoxc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmjlqjfa.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nypqtnbt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vdljcrbr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jiaamywr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdmidhfe.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pazcllio.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2imsdojdl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgrvslrg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xbcckwoy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zelnedtn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zlliiktg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fvpdemkv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2veyikrsq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcqysnke.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ytvangut.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ayrgfslg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rztfmptv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2btkicyte.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pntcobsh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sfnhhtxa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2pgdczgar.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2cftwmxqu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jgccjqdu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rfnrfafn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ttfoqfxk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wvlnenun.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ftxnaszm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sszxjddz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ibzfyhxw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gmuumqdh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2euysdrvv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2suovxwvm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ujnyymgx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fwuthzql.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fmlygrxc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nakxvwqo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ifdauuis.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oicmvcwq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uhdvzauj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2grtkgtpi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rjaqfcve.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2yunsusfp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gdwqygbx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovvvowgo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eagqazqo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nbkolzvz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2khsetjtg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bmzrzhjp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmyschtk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eztgexhn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxhaxqjp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vncamrwm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtwkbyhz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xoygjzpc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2epcsjhqt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2eyatpfkz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2giprbuxn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2sqmfcwkr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vsquaulp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wogwcvyq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ginipxhp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2utvyutcs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2pvizpqmi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2iyiusxga.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qtzmkdax.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2opespqdo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dffpxvkf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2awrnqqgw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dtdxhgwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzrwjdff.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2oolzuxct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oghnlyex.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nchwajkl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jevohwwu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oipketxt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ondlgzpq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwiocqiw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2gfjylbdk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fdlkgucs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yunmlxvl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkpfpgea.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2butlljkz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tnwjznwt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eaisknzq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvdqrdec.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nuiunsml.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmlmggfg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2afuvluaw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2viusvhnk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaduuiyr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ccoswrfk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wdfexfmq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tymqdetx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vgpwhxde.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2lsfmmtpu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2btxkomwo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tpviwjvq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zdbchhxq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2akmsfbpb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ycftjsod.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pwtvciis.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlmiuffl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptvaoqrw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzbrermo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pebhfuij.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kilfuxhy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2otmvtshs.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2getgqsps.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2nisbralk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ymqvwxrd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ccozooxo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfrtnwmn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rczddnuz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiatvfjx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wmnpmcgq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rosyopqq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2mufxjvat.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2oxzkauql.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nnpxnhhl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aptlbzas.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mjjpwviw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bszmgvjn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ueegkoyw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2brlsuwko.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kpazfbbn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2yxgaukqo.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xtasxycc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kqurtqcj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lzkkutjt.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qfbddvzc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hfpjqlvi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zmebyiwg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2imvwdlvp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fsudfcnl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ikrpfakr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2mjhafscw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2sldyuata.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2avwrngtl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dpryusaa.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2sbslkqiw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yurrtygw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2szlrxsvj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fmwxoimn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zasmqexy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2eobxbxtr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lvtjnamo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqgslkha.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jmyrluup.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbuisalq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrmaiqwc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2bvvmbvbr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qnuvtfcs.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzplkonw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2cbdgcuhv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rnaeixlt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xtonnfjk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2okhvmwke.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gameludl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2otmrswvq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2krtbtnic.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gczrjavx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2thxfxdug.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xgpzluyh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nmoljlat.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwwfkjot.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yomoolrr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhwincsr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2huihipya.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2psjezqeh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2khnymvts.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2baduguuf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2apooexju.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bbttfwzr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fjczqjca.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tevxtrpf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bjxdynqa.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2osmxcwiv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ztwrrwib.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sikjjjwy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fhbbdtfb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bzisirbz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rfnjzldq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sicddpbz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kwmyrwct.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rgkjkgwu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2medwqdcf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tnahggsu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wdpezuos.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2foyhaeyt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2dhsqojma.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jzsrjnvi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2oocofvbz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jbzbxggx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kmbkhznr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujdlfaoq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2juvhevxd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xebnzwpw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2brhmvuow.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xvcjurog.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lgcflykw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2mtihdunz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2letpkuhc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fgcvdoul.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vnehwsuq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jsbuadzm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2sjgmmagv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ojtsoyqm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mvgjbmyo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2yjjxlqxs.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2uojsbcxf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2olqyxmkn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mcqjmnbn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kdtwwvwj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jaxniwjk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2yzfwmevx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mevzsqyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwhsijrc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2dikgpvko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djnxigmy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2fngqjmad.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2biykqlik.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2erzpqfpg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxpuxyvr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wnwxlewu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2khgmodlp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wcagzeoy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ujzjasge.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2wqygsclx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wumgoxqk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qujbyewj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ulionnlm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxuvacbm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwuoxkvr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2etrklxbh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pbmggheb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cyuqgxwo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kowmfowp.html


<!-- 参考信息 -->