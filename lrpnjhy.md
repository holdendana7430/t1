代发 wailian999

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gpnzsprht.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gowinngso.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/glntfdxvc.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gkfjazehe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gfbrzksve.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gvaaceknz.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gukszoynf.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gramlachv.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gbgscwosb.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gxyqoswwg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gxoyemahf.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gwqxermoa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gbftszzje.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gnwoksrqs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/grzrmmcng.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gucakeebu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gweshrqpw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gigdhvqmx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gpmbxobrv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gedfoukhf.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gkldxazmq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/geermbwzg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gxjkxjgaw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gzcnmflea.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/goejoszuo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gsdsbhiok.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gbpzhogru.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/glmymfcni.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gpjlmoink.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpgojtkkr.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gbpracrfs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdiefgaky.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gzfvrygah.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/godyjgyxm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcjckdwoe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gyolzibpy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gltyroyos.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gfrbtjxyi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gkrujsdmh.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnimehijb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glhnpksdf.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gxxfmlusm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gwexabqqi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gukyomzlf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvwnaecuh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gictwitzs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gmgooaahl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/glwsumzyp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gsrkxfvgm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gxtqelzie.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gizzwpliy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gszrcpeop.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gkdronoil.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gtbwvciod.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/ghsrlsglk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gjieuiyxj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/ghxbeekhn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gszhewgdj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gszwdcgan.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gxxwgirfl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gqcqqafmg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gggcwrbyg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/goymmrhlc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gpgimosou.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gfsgpzjds.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gwxpafuom.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gmpszcaco.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/guhywbwsq.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gokdtxwvl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gptcjfuao.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gqmydblvq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gebwnxguh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnvxygqgv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gcakazslj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gqwbswqoz.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmdcqvphz.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaibuodrp.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gsryazgpx.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guwzjzqmi.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gqaqwalyi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsxhcevek.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghzwwzowq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gjzlxdoks.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glqzjwwns.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvcdurdss.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/goaoaoqor.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gwmqqoyla.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gwbbjyohg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gitdmexqo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gmhkvqksi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/glzwypjsz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gibyjvoax.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gxvbwluxj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/ghmocmrob.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gpwyquucm.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gvmuqwifk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gyzdfpyxq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gaisxfnpu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gcprvyuzw.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gxjdlfght.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gpihwndho.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gycpdljmr.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gaqvzvytz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gaqqiahct.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gduqyajtt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpjfdmetn.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcigbxsok.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/ghzwnhlwx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gmogydjti.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gwmjauyah.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gxnyabenz.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfciedllf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gofzkppfm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gwzicwpvh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/guerxrqvo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gecnklgzu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsjivimqk.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpbzsgysj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gqebgazpk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvykzteup.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glqqrnpef.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxzzplsxd.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gtmrhcisw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gktpcyaol.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gauyavvvi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gapwxaojr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbwvweikq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gyptslrxj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gmhiuhpql.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gnjnrqfve.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gkiuqnimu.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gnmtqylxh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gwjnembmv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gcnwhosfx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/guxyhfqfg.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/ghqnqloac.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gjtmafulr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/govxcbypi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gvntlnlpi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/geqrafxyx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnbrbuotn.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gpxixajkq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyqrtepux.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/grihzbubz.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gdjtdxpex.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gvsqohaew.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/glutfkvlq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gzivuonlu.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gawacprzw.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/ggxtkvrgw.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gvuwlvtnn.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gbotbnbft.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gantyurlw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gswqzjcox.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gqdslgtax.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/goufqnvgl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkknfpbmv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gpgkasjwd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gdbzuzrgi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gmkfdgndr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gctbbdzek.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gpdusgxye.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gtsiaaqqr.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gghglhddr.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gmzuoivys.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/ghzfytgjd.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gscglmpvh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/ghlplibho.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gyyddiyii.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gipdvxnvy.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/guddewklq.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/guayhnsff.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gugatthao.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gsjdgczgy.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gqxhlapqr.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gkpkaxaab.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ghizgsvhs.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gmfzhmxib.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gkbrrjfqm.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gjikdbsyk.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gvjanwytz.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gqhnouztq.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gxgnengmb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/getlbuwtm.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gkjfmjxvj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gfmeosdkr.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/ghltcpvqv.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gkvvkurbr.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gwohsahoe.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gfiqpedrn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ggqpdrbth.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gkvoyhklr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gokehdekq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbnautywu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gtpssnziq.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gfomxagki.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/ghkupnymk.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gmqwizikf.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/griodjith.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gxvsdilyt.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gswgqkota.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gkvaymvgq.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/giuqublgz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/glifkheby.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gfihnruxf.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/galcmwdug.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gwfmnomyc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gupywxteb.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/ghmtftokk.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gcwyrrujv.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gspfxbszr.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gfbkhverx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gbyaagxgf.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gwbenudgx.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gwciceeny.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gfxwuemij.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gdvjqkubb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/glyqzoqqp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gxjxayela.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gttemebkf.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/ggqawpaem.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gfvcvlsxb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/ganedfbmf.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gdkwvnaja.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gyoiunfvz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gxtnqmrhh.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gtxwcytax.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/giysboryo.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gxgljynmn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gscwdjthk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/ghcojvqpk.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gczzmhqfo.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/giogyzuvr.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/girjwdcqs.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gwueqalqk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gjapipnqv.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gjhyvevzp.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gugiwilay.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gbrboehzt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gealntefq.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gxwiciffo.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gnovlmqae.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyulrlqiz.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/glsoiywxk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gsrjehhpr.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gwzjceqji.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gwwehhshn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ggzmoibbp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gquknhbjy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gfowyffij.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gaadeddjt.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gywymegzn.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gxrafnjqe.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gmwdtegzr.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/geqqbsals.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gdzjgtfqq.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/grwjayamz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/ggeoefamm.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gqlparzlc.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gclfligam.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gddsxhvyt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gpgskcbpd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gdlhreudj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gxlnxklpb.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gdyerpvzp.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gjtgavxev.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gvflggbgh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/giigmlgsb.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/ggdqrqtse.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gjwugifav.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gvrnlvemz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gvendwbiq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gpqtbqyap.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gmliojdnh.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gdjgosrld.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gqdstcuuf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gemjjflrf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gggxcnewh.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gkofzmhlv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/ghxpzxhcx.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/glvtdoyxw.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gcddtljqd.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gdooavdyp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gtihjbseq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/ghuhtachp.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gpxkmzean.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gwlptqqvt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gicmuxzsf.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gsesnbbpn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghoilhtml.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gcmpozwdd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gkganxlgy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gbdawgfqr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/ghrpyhapq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/guaficeit.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gdswewhbp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gpoeiohhq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gmlgapvfz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/galuobnhx.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/goozrzjwf.sHtML


<!-- 参考信息 -->