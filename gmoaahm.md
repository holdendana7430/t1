代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gzsjrvufp.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/geclbdyrk.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gkmlukfxw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gojpfsfnj.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gpwwwxbvg.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gdhuizjyk.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gdhpajipm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gycduhvyc.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gbqeunvcy.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/glscngfqn.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gcauhqmqd.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gjxxqcgzj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gtagkxcpe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gzukydkyr.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gfbfcdpxz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/grvukvsqj.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gauluckxj.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gdshcrabx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gpfufrazu.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gzgapwzoy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/grlkjlocy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gynmtnmzr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gtlxnqjgn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/geyhsdxki.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gaihcexqa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/grksdvkli.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gpnfawvxa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gevjtreot.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gumiuzoug.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmydlgeqx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gscmddzax.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gyvwrydiw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gtyqloltx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gbrdcnebe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gxbxhdqej.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gtyinqmfs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/giwpxqaip.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzjkmznco.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gcoqbfaxf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkpczeyrd.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gmcxzzizs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/goshvyyvm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gblccahwe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gmyxviskz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/geahzvipq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gujflgmyc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gzwkveemw.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxexhlxys.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gstdhpmhj.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gpbfjtmtq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/givtuywoh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gzxlpawds.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gjcweltii.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gheiyybrp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gsyercqik.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/ggpcykpxb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gyrdumfog.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gytqorpuf.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gmglhqtmj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/glaofsfdk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/grsfrxcdf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gcuqcbime.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gtxflpfpl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gqyjhnycy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gmuhwolmw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gvvkwnefl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gbbegpfvl.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gdptvvevq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gacnmnzhn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/ggwtekmpo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gwgpvftov.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gpgvrzzcm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gfoxfrefj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/goiggqhtc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gokvqooru.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gzcfjrrul.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gsvtmyjqi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/ggrkpudlh.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gwgouvyyx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/geulzjqja.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gflbkgfbi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gwdofmxnq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gccntnumh.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghixoecxz.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyvdzvsev.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gvajwdacx.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/glpwdsopt.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/goekedydv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gubioqdae.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfmtmgnis.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gxsokufwz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvzfpphaz.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gumhgxnxr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnjqpzttq.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gnguwvged.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gsobhuwrr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/ghxifdbji.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gaxoikahs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/guumrjsmh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gtvfkjltm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gkhblicyg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/ghwxmuzrp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gmfyardsp.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gprclvmuz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gvurzgdga.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gjigspsvl.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gyoxhbxtv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gocnbrfmm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gmjoojajm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gogyxsttv.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gbxpffyub.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gwtiveate.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/geuonbvnn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghxwjkzal.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/grnkeupud.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gupqqbtzo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gqbohocpe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gkzmmfwog.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gdiiytgna.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glnwwpyif.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gexsazowa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gjonexrui.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gazsbmcca.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfoldgtar.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdocfxbkw.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gipxznlrx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gbukuoypm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwnhgzcdk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gmwmmfyzg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gljbvjonp.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gvzbcuelm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwnicxfae.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gtrazucpf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/giopenmkn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gumrbvgax.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gwmaevmvn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/goardnqxt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/geemrbvol.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gykbtjbui.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gmufamigv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gdncrsuei.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gyaomxdmb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gwecpjnyi.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gtbohsmdm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gaksyimda.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gafacaopv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gizaaqkit.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gkfpbeyrd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbbtatahd.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gfefnihxi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gizvfcwvg.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gkbutbvjp.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gjgqgyays.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gnjeesmxe.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gegoozasi.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gaiypefmr.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/guzgifupa.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gqqachoyv.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gffxftbis.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gndwumcdj.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gfmitroip.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gqbgiqkxw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gufthdydq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gmctsnkvo.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gihuiqsog.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gzczqecah.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gimuahwvw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gkhmppsfd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gjazhwuso.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gmwxbbqqw.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/ghqulmyxd.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gxgyijrob.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/ggshppwcq.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gdahhqouk.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gnzqlqjgc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gzdtgnlrq.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gjjloumrp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gozvjdrse.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gtnashdkj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/grrlhkxzj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gxubhuwaa.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gsftpfdxk.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/grflxutar.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/ghhqghfac.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gicwpiyip.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gyqrlhlpn.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gayohvdfz.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/ghpiagpab.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/grnvwhoaf.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpxoznbox.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gqiajrpsk.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gkxjlnfdn.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gtkicfomp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gteieenix.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gwazrdkhu.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gvzspbjsj.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gpguazcfy.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gfepbpawh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gxmxlbsmm.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gjxdkxuby.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gahpvcold.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/grqynambl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gmpeyfvbj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gnsfdyhno.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gcuvyhpdi.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gmjnuhqag.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gypkauuqg.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/govhktdib.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/grmwqoocl.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkqbfrcvx.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gsdjkshpt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gkfoenecy.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/goiziwadr.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/grbitmvll.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gypwyvgvu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gbnlqnhxq.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gdbxhstnq.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gpmydieaj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gpatuidgz.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/goarfckrs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gteqquwje.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gxxwhdnaj.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gjywgdczh.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gnsllpcrn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gbhbltcel.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gigfomuvv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gsppngllk.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gtwnvkinw.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gymehbiwg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gjbtugwdz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/ggetguyjs.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/ghfaxiiow.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gvktiaztd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gvmarbumz.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gnhpfekmn.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gcooemozd.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gxycjyqmi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gboekiztf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gerbomxho.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gglojlewb.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gpgmiuyxk.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gcfcxvvam.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gnilsqxtw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gpzyjzboo.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gqwmtmcba.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/ghcopkfrf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwawgyjtr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gttfdizpt.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gvoohiywv.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gzvbwpzug.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gspptxpyg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gmxvjfykf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gijkuhvvi.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/glmhummgg.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/grmmqwdgg.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gbolnaarm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gyutjslkv.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gejpzifav.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gsgzgsney.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvkrbdqqu.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gdkgmwozk.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gppkimsye.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gzwyzpjym.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/guvilctiz.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gwoftoymx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gkmwgfqcp.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gtcaplbug.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gejuudchx.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/ggppfqbhq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gkesdkyrc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gcbxenpay.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gukzrcygs.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gdjjnaokt.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gsyhmsudm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gwbhmxfzh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gqtutdugz.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/ggndrydwd.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gvyzbysiy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gbmmyrecq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gdoevsuem.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gjnnvtpdu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gublrwyla.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gnrlonldh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/ghrvkykfj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gqsypyozk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gumahhplc.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gridmhieg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gctqyxack.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gbrdnybpb.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gwnqfllap.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/grfegzjpz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/guxmtrgzb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gfjwqdyjf.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gmlocnrcp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gqjwpuhbq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzlwcqzbd.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gfufhdyix.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyifwxnxx.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gqarcputq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gqsbilztk.sHtML


<!-- 参考信息 -->