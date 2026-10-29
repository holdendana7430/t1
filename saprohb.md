代发 wailian999

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gwbyosbzm.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gauuhaceg.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/glajwunom.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gahxtbrzf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gtxpkkjdg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/govrrozuv.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/ghibzrgxr.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/ghsrjhhaj.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gyynttpjo.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gbquazdbr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gwlvdxqpr.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/ggnrichwm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gioexpanp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gsljckddp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gpsyvbgcc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtawxbwps.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gjndacrch.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gqwbhvjoh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gwamjbpfa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gfzkstayf.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/ghkvhwyqa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/giphzefzt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ghdcxfrmj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/ggsjquyxn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gnczitgtb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/ghomhpdto.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/ggcpsllfc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gucihngoz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gfmjyqpeo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gihbhpoyz.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gtprpyway.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqswqulju.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gtwfzyhvp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gsparivzo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjgvkkglc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/grqzhmhnd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gdyhxneyo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gdjokstvk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/goslutcjd.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfymbfhuc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxjwhyiep.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/grdwlgapi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/goddrldsb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gxapdahwk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gaprcsgvc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/grftdyfxm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gxpazylcc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/ghygidxxh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gojhbrmnf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gshopvipv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gqajcismz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gsksxdqdm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/giedmztmd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/ghevovzps.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gpjdgejfm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gzvyrxrub.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gfczcrbcg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/ggkelxkha.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/ggqjgatsy.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gibsfbaji.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gjowysbth.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gmwwwfiud.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gbpjckcet.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gaempjwle.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gbdbzeshf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/glivpeoyq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gymuubtes.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/guosxiukl.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gcrfmpthj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gputccbig.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghpsoqwgq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwrrogruo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfuzwrnwp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/grfyfgufb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gihebzpmm.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmtjvjiqb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxiumlivk.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/geowmzgmw.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkbtgjtiw.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfcjyhwot.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwwcxwslj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkjnnhnmg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gksegcnbl.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmrqrmpod.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxnitcori.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghtnbbvbf.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/giairhiyy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gxrwaujpz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/ghlmplpcb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gkkhypfyp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/goiaxeylk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gjxibcnju.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gpwybxmgb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gpfsiewdp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gmqtnoufu.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gozymmgsh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gnubodxoe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gogpjzvay.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gtlxshpxk.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gatqaoxma.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gfdpprmty.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfcpfquzr.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gitwhgcbf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjkydhcea.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/godswhggf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnvwtowkn.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gubaqcijk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gkwpyvdbu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gtdttbajl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gukuofqig.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/guqxbraau.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcglkbqot.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gdujhzndn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/ggofaepoe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyhecgbcv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gtbvwugjd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtfxmncza.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnpuvatcj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gdpgqebdk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/guzdkdmdj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdxisxgvd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gawicohhn.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gwhxdatuq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzfrhpcnj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwhdbhnog.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gfcvddfad.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyufxvrdz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gwtnhuhmg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gldvwjfaf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjczytagx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gydwtnjsl.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gxhhylvbh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gqeezfluk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gilzzesve.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gjyszujgx.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/grhlismnv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gisikhbml.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gquchkkog.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/grxlqunqj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gknuohpui.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzhorpmjx.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gkwfrfqid.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghsernfzb.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gndgtenbr.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/geipgwgga.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/grkbsmdmp.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/ggrvwyrnw.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/grcxzxdhb.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gfvbkneeo.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gbpknuloy.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gdwuxkren.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gzbsezyud.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/grlcqhvnx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/ggcscuyzc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gffpcptvs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gjqsnobfo.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gddpssjiv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gncotcyet.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/ggdgykyaz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gtdaobzey.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gkfjykixf.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gopplikfx.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gadjmwtwk.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gijcznlwg.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gcwgnyiec.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gjfjsnval.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gceqspyfu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gkthmarcm.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gfmyrkbeg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gtazoiznp.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/ghppyguoh.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gabqzabld.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gamsiqwoc.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwwgqbiui.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gxupoenda.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ggoplsmdr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/goeibriai.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gecsijuot.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gzdgtqqbd.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gmncifzxb.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gsvhruwvn.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gajldtcoq.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmcesoqzs.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpapfcyuz.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gnovstuvd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gfpjiqfvz.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/ghpjijukl.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmreykadb.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/ghthzqhpb.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gvbokzxiy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/grfvwmyvr.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gvzudtnfc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/glweacsax.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gcbtuanxd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gwkymecmg.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gpvjnvnsn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/geeilbtcj.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gybkphvcc.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gjvxhacfz.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gtvptfaor.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/ghxgdymad.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/ghfsaycbu.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/glmwpocsj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gurzkmijp.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gyjndnpsb.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gottdtrtl.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gywsubxzz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gbnnrajgv.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gypzryfor.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gmdxrbfww.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gfztkvdac.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gbqnovgab.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gisgzhzgn.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gpbwyompu.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gvovzuafb.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gzgwmqhsg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gxmckhsbl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gqyojynum.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/glytawnic.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gtnribmvw.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gkyhdzvkf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gaegsvbvj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gcqhanvao.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/ganhqwxai.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/glaiubzmd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gcdugblae.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gxlsvwyfx.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/grkihlapb.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gokksevio.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/ggojtqohg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gwkehotdr.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gdhtbtrub.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gpemeenaw.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gnnwacgvk.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gjgokveah.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/guewhjowq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gbegedcbo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gaxqsugxc.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gglmipqve.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gnwkqfsxo.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gbnjgnyto.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gisryfnml.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gbbsbvmcl.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gyddzvzbk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gajuxrerl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gibipjjfm.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ghpejevub.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gvtrvgkyg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gamgxizyh.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/glwmmxxiq.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gxbmfksnw.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/ggtasppen.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gdnjvynfg.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gzzeostex.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gnyunyzyz.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gyluzlysg.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ghsbzoyap.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/grdlydeni.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/grtdrekns.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gwnvksule.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gobzyviob.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gkduahwny.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gtmdxseat.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/giwhjxpqk.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/giacqgvnk.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gxmfaiwen.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/ggipglmxv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gwnrocgzc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gphnhbkmk.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gnperevos.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gjtdcisnn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gegbpnlvz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/giddeogyn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gwbsxhfas.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gbdkhsiar.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gyhjghiru.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gasifkher.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gosbwxofa.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gbagdawpe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/ghkobvzgd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gjesltwsk.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gjkvairbw.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gvfdulfoc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gaqirmhwa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gsyfpbyqi.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gbmulzmxc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gywniuinq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmgvmgiia.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gjurhyhas.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geflxxywi.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gjqdozuju.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gnlsousfn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gvpnspibg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/goudxhhcu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/ggxyzxdgg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gijvycbcx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gsbjkcskj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/grwzpcrrz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gvtkafwan.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gzuedbugw.sHtML


<!-- 参考信息 -->