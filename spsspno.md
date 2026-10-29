代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gfomjbkla.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxyvgpnmp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzdrnrja.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/guycgbygq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gyeojakxg.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/ghheqjitg.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gnfbpgvnk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/ggsdmnbba.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gpgnljdde.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gzigbsrsa.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gtvowdulr.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gdgzpmkuy.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/glaipcrgx.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gdleofbyb.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gxtnhjgwj.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gkepbybsh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gtdkgbgtz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gfjxreqsm.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gtjgthfqd.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gufbscjvu.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gpzyybjvb.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gvjqjxzth.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gawucvpxd.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/grfbqrpos.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gttujkzcy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gguhosknb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ghbljyhta.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqqnsgisn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gftxxweba.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gxuzznern.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gifcnrzgs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gpbvkfgqt.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gzowlddhq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfudznfkl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gblfemyun.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gvizjczsn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gaqdneiyu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gyqxphpwy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gikmknydp.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gzdvvlqto.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gswhqivou.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkrsamvzi.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gyspgzpyh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtfldumxj.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gumlyplns.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gbepizovh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glieicacq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gbjyltslc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gqnmqeukj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gnknbdbrh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gtlnxmarr.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkpyexanb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpurumzvw.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gaowqkzim.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gtnzmjgpg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gfwxmayvi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/ghfebvvnr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gipqsovon.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gqbghcxqo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gbpauzdyi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gyytrktjd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gogxwmzsd.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/ghumoybsc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/ggovlioer.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gdzuulmev.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gkuiveazc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/glngkocgs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gnqkpftys.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gtqnunzmn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gjoeuzygn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gcrndeulv.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/ghwzfyzyq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqsarkuxx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gwmxcvwmt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gbvztxcci.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gkygttytw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gdblgipfh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gigtsffcb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gnsehbxof.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gorfvfeim.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gemocqwmi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/ghlpdamhc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gujjxocvp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmytviaus.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gduvgrabv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/giylygkwc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/glvbwtpzr.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdulabaey.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/glfupqdkp.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gvrzyspqf.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxedqgvoi.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggxjorqag.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guhtuiilk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwdwiajmt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gwwxtaggf.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkphsuwbd.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnjmbeavl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvweamusq.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gfnpddmeh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gwcowtuvj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gcnqvtmmp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gaqqeokik.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gxropyemr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/ghzsakqiu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gmritfyik.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/giwswdzcq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gapownesk.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gyaavoocf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/ghqdsvdgg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gvaajdwmm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnzkvqqor.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gpygmdeoz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gtxcvtpdi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gfztjethw.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcsllzqzx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjphipqtu.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/glppwilfc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfuooduwz.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcewlaysc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/ghmkytdoo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/giiaycrys.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gxgjuhawh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/guqoouqld.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmtrofivr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gzjgcuzrn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/glrlrxotz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxyxegpjl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjfjkdlrr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmqpsgpxh.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gipeaxdgw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gcgtklqwz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gcijhogxn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gboeqnsfx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbnubcxcp.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gxlgawnmv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gybpubdtt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gevffrrqs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggdaskasd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gcvtgtsty.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gvuwzwphg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gaagnzrvi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gglpexkne.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gfnfgxamv.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gyxeukzjt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gfvpcozic.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gthmbdqbc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gpwxyysdw.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gorxivzjn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gcequoese.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/geljxhrfb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gbekujcie.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gmggrtnxy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gljvgzckn.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gdubksdiw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gulysridf.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gainyxqjc.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gvpwsusup.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gmujxkujv.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/glsvvljbb.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gcxfvlgyv.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gypvyukun.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/glfhikfvt.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/goolxzcvj.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gftlcfqmi.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/glivqmetw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gtxwwqgbp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gwwgcenlr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gporcloqt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gibgpinlr.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gxtgbvoiu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/ggjxbxjml.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gzuyprqkf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gmymqgdww.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gjuwrtrhh.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gdcozegdr.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gkznrbtvj.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/guxaxfppl.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gctijrxhp.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gfzrxyulp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gaywrghdp.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/grbsymber.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gwrkteeng.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gconexpmc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gdmjpemyp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ghhjkptav.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdceyfpon.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/goqlqzxds.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gkrhgjaqj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/ggidokjda.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gzrlytsvl.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gnbzelqyt.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gxegeywpw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gpovkgene.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkgevztvi.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpmfdidqv.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gpzgqmedj.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gpkvbyzbu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gxpqngbbq.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gqcpljujn.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gjrgoxoar.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gblhiquct.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gapeuqlxn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gdbsljvrf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/goeivckim.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/goyzxzlhy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gkcuftvbe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gurgzwund.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/giaqgbhue.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gfzknqgud.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gjsykamax.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gaqhhpvel.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/goywwoavq.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gzzkflega.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfobtnoie.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/guhcjggic.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gpotgjfbk.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gxshcgzjl.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gfvvzxqqx.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/guvvejmel.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gzzchwsvs.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/ghpflfkpx.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gxiargmqa.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gxomhxtxz.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/glqeuqzcs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gogatqpvy.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gboglbezq.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gkmsehwtl.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gtyprumim.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/guabmnfxw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gdhppstme.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/grvxdztdy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gljhfumrc.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjlozquoj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gkwfkelpx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/goexfjmkr.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/glhjidulg.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gklunicbs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gjbgzgsyy.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gerfbuuez.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gvmnhldvs.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ggikwppdh.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/grhzygrzg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gtgkessrf.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ggxpdqcqd.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gbuewmkqx.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gnaswdxak.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gowblvbji.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gthsplzry.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gavhxtttc.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gpzwdtixu.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gibgscump.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gztncxirg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gegherksz.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gaxmzcdgz.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gtmbkgaxd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gvalmmwvq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/guqwmsvsg.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gmqcsnarl.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvgvsudxu.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/grzbcgwoc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzdlscqle.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/ghgasjtjs.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gwmqvqhyj.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gcumwiohc.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gdspwebzp.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gehflhzzl.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/geopzjtqw.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmpgsxofs.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gdyurikiz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gzumulkml.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gvncwqukl.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gfwkjxfjq.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gkjvcoaso.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gsuzhiyac.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gmqwseqla.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/glykohaix.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/galdqtvuw.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gtgcmbtky.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/golswybqx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gpdrwzzcw.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gfznnqahu.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gtocbljts.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gbgxsswyh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gkdfcdoaz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gehzwpjmd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gddaadvlk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/guuitpenb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gridmvzqe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/golnhjytd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/ggyzmufzu.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/guwdmpish.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gkinnbcll.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/ggfqfhhty.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/ghoogwnjc.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkmovwzgf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gnyilzymd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gdvfmzyxq.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/ghgursgrs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gnclcvvvq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwhmyttiu.sHtML


<!-- 参考信息 -->