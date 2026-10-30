代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gqpcjqaaj.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gnarvkvlh.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gatfodtaw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gofukzctc.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gxbituciv.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gguhxjrjo.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gluqyqvrj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/goxnnmnbc.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/ghwqaauof.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gycmkbwzo.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gfklsyamk.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/ggwummrpf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gsjwngjzs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gemyibcfe.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gcnzxdyhf.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gqwrymvqr.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gdhjnhpur.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/grppkjnqh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gckmauisy.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gpfalhwnh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gjpaowwjg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gqbumtvml.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gswuzsoog.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gnvygkfia.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gafpyrrza.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gkaueqbnu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/guklwpelw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gbrmikjve.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gphwvlvgf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gpgyqeuuk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/goybdbave.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/ggxlydakx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gsfqrovce.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gskywfsye.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gwbsoxnwr.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gghpfefag.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gbetsyzxf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghprrjcbu.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gwnezeerp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghsuhvhrj.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gpnirimte.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gagxsesxn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/grnkzbjed.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gbublzwlw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gkpmbsvef.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gxfiozthn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/girinbkep.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gztazvttz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/grceqokzm.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gpmxtirdc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gyjjycotg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gjqenaoqc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvpxlvwaz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ggogcqreu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gulkzzaqv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gijxsadsj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gzyxrjcea.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gdaeszpox.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gqaavcvbp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gwzkxygin.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gxfuxrxch.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gobwlsyjf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gdhykkork.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gowkfevck.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/goutaxiwz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/ggiixxhoc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gkpffohxy.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/glfzrdvsd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gduvhcbac.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gjcxftqec.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gjgiprweu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gzbdejvwl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gjahmqhbu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/ghtfttcgf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gokfmqooq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gpofkshtz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gwuommanr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gwprffxjf.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghctlvxbz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmgbcmefb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grccsdjjz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gyytcsdsu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gyadjymst.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glbusuhba.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glqlnkufy.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gypufajya.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxqrnbibr.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqndhhnzu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggsncrcuc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gznmxewtt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ghglewulm.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gexsajjnu.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gytbpkivm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghffpuagl.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gcvcnakor.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gwuorfaqd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gxelsprcn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/grifustnh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gfdcrmbdr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/glkcworyq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/ggjcthilg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gnvfowclq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gonawbqlw.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gvqmivnln.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gfzaydugm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gxvbkqhgc.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/giojtlskz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/ggjlwqdbc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gysbbluel.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gqzfnsbzr.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/guyqiubpv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gtmwnoudf.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gwbmftwyn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdfnwmjuy.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gygqiypii.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gaiudmisx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gueogjklj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gtjdpfnry.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/genchtsgm.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grkpuxkgn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gqeeyprnj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/goinjxykr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtazsooyj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvjxakoza.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfjenxgaw.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gunchczbq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gzajxldhz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gdmqyyzoy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gavwscaps.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/grndbwhtq.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gajdspzsm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxpnibfqp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxvyykuyh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gmhppsdcm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxmvghglp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gkixcqubi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gdganwayj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gomgnvirz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/ghdnowcza.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gwdvmoimf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gvoxzqykm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gbemnnblh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/goickgbbs.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/ggukxunty.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gobxlpghf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gyiskfukf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gstaztdpy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gpbxggdnq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmbwgqiab.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/grlqgngiv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbuqjphuy.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gatnhqalu.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gymdjbptv.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gbhtxihwj.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gmkoqblde.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gcdaqekci.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gbalixwbf.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gsduqeegi.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gvelcdked.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gtuwvhnhk.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/grocjnrqz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/grlmpmidd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gfmweoaxr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gfbauxcbh.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gtkeusmaz.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gohyvuauz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gssytdufk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gzlpmbsye.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/glenvzhwj.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gnmkwemhx.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gusdyuydc.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/ghjaxsrzc.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gurbzoqfi.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gcvsmxkbd.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/geypkjnje.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gmwiadplw.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gnvgpafqh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/grqophawt.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gbjkifkzn.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/geqzdfpvc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyymqnudj.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gvsskkfra.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gyujhrssy.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gfagijtof.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gcmpqpdpb.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gzkopatgx.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/ginppguul.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gzjaugyls.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gkzvzcgqj.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/grdwhbqzx.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gtrwumwph.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gugonljaz.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gmkqhfqjj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gdyqummhn.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gajddbxsy.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gtmxwpivy.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gyhknfqye.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gajouutqq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gyrgpsatp.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gjbsxevlk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgffpji.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gbgsnydhv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gkcmegkha.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gsngxabrr.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gyjhtrhvo.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/glurucrav.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gfhfllfop.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gmlqmhmru.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gpzcuitxn.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gfrynsjhd.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gxngvyqmm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gufositql.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/goglnatke.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gkpbzugov.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gnunxgtjl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gqaagtyol.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gpsnpiuyn.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gxmjervxm.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gaeynznmc.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gnilfvjsv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gllmgpaer.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsrrlkysj.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gkekbowqa.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gncolchxm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/ghgkbgcdv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gcjedeazy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gbaestevl.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gcdhrvwkt.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gbbwqwsmh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gzniujzod.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gdidsgfkf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/giwdfkpka.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gzqlzfjub.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gjwglbwkf.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gwrfgfjgm.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/glxrzyfgz.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gnsgjovve.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gtjsixtxe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gbrrduwar.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gyzjiqyfc.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gvdrknfae.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gpkorvbok.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/ggoewpuun.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gskyvdbzh.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gowfbbrgc.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gxugtrpdw.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/glrqlcqcd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxlwjukab.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gxzbrathi.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gwdvvrcbl.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gaozkebju.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gdkebvgkh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/guqeftftp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gtqhlxtcy.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ghktdmiae.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gqmaxhhlg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gaolswlnp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gofzhjbcy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gojpiipqf.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gytbhlcqi.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gmcsgmozr.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/grxtmatto.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gawnatejx.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ghzudnyab.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gsioaxawd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gfqcxtlbc.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gwiwguiek.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gakeaiios.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gqephdthx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/ganxmczhk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gtkmgjvgd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/ghgwiwpby.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gmpspntgj.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gryvkijcl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gpfnmilfa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gwsknhunq.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gryhyuhyy.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/glnijdhrk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/grojpzzue.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grnavkbfm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/glacscaum.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gpwkegdtq.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gdscjmfcp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gqpfmhivi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gjqexnadz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gyqzebnji.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gjrfvhbsd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gmsdqvfct.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gpdhiqmia.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/ghrcoshwx.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gfbejyqut.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gbcpxaaoi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/guaohahct.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gxyqaumgy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gidskkdeu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grycmavcx.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gvhcyfiwh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbdduyzzq.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/ggzfcvrwz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gfbkrffuu.sHtML


<!-- 参考信息 -->