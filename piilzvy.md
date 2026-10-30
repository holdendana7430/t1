代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gawkumdkt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghyfzdgqq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gkfhflcdb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gflonnwan.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gekinykhd.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gygcsodjp.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gyicfijks.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/glcfphspq.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gbymnyhzw.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gxtjweesk.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gmpykzblo.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gpjswpyvq.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gymkmzdop.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gdymzplaz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gbsfapoza.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gobiipvkm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/glxqubdns.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gzcbuanfd.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gczvgaenm.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gofyfifnj.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gqfoablim.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gpygzpnbt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gztlekitg.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/glyhqmhvl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gusqducpi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gvtqjqrck.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ggxdmmzuq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/glaerbnja.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/glqmovsvo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gjpjustep.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gnhlofdmm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gezninejt.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gcrwrdmqa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gjvbfommf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gvjqqlenp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/goosyfwfw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gnzcycyzy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gryhnxycb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/golbrpipk.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gdtklrcbs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gcgafvaif.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbsxhovuj.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/giosvnmvc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gklglfmge.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/glxerqvpq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/guwjxwtqr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbovexzku.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/grlpzepxx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gjcmsvaqm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gzgdbxjve.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gkayxnfzx.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmauirwbx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gamdbkvqm.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/ggbplqitc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gkmwvjowj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gqqimejuk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gqintwcwn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/ginvimyku.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gsxkxbmrn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gtimuguor.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gbxlxkfry.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gbaorijmz.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gckruprzg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/geyokegov.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gdnpyspux.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gpuvglvjx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gexkamaol.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gfbvidmiw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gpasguges.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gjwwncuid.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gpxozkntu.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gxlnrwgbi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/guozkjglo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gpywewbdc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gvmewpbgq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gjquxcqlc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gkocobbpy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gwpdezvzn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gkzvsitac.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gcqmfaflm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gfrjoyneh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/geerhgnhg.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggzvumdkt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyylihjxp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gijjpqnwv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/glslyozot.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gcwzebzrr.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmvryikva.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsgqkvrkf.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gyjpvmehj.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsdtgkxgv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbypopbjc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/guizurvqv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnihxplst.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gwcvpvgsr.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glapewsli.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyalebaeh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpocqxbkr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gslbhyvsp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/ghrkyuryh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/geurnvxeo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/ghpjhlnep.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gaxadsrmv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gwsyqptfx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gigvivmni.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gxctdowaj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gngajmrzp.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gxbvnbpny.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gmwszzaaz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/grvsseaex.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gylumzqte.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmdsqvglk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/giybaywiy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gowdlosmk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gkknuxild.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gmvvekvoo.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gczyzknym.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geysyhwdz.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/garnaaaik.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gahmhounr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gnmzektrm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gvutlqaic.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gawgbdqpm.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzbvzpugd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gnjakkyds.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gcbjuphnl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggjizhbmg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gabozcygf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gaxjbhgig.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghewpgrbk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gbnbfzsxj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbwkafget.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsegbmlra.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjtxfsgia.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gstbvfuik.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gjjvrqmzj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcqjzrxnj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gbdjpdoll.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gdsshkvvm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gyjoejyrc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gdbodxudu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gbxdhxjax.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/geaqyeibc.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gcyhzifsv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/glsksftxw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gvyocvtgh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gmxwpctfc.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gybtfvkgf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gytfaatsb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gpltxypkd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/goufzayhb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gpmgsmxjb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkdjnuauc.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gxqoprpfk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggtsiytod.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gbzbzmymq.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gijwkclno.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gmhqlggje.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gobqwvygc.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gwjpjemvf.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gxybmogto.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gqifhwoqx.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/ggkievqih.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gmjhibzpk.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gwtbdqyff.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gvgaufmsx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/ggpgjadyb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gwkeorpls.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gffpblikz.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gdodrffkj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gmzahokza.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/grqnvuajy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/ghpdoblff.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gfqqymuzd.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gwpdwtbuq.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gvhlxeqdw.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/ggenietnf.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gvdesveml.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/ghwawixoj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/ggzjrngdf.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gpaxrdwqs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/giyiwgwlo.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/goxsrujse.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gyruymjsc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gnzhbspix.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnuymxveq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfkpoafs.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gxujlykia.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gtxrkause.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ghvvfxktl.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/glofbesca.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gavxdanli.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/ggzmbvegf.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gqaxjesqs.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqagvuchq.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gsmtkqysk.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/giirabgdm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gqgyjydmc.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/glgzldfyc.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gdoevokux.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gjwgwxsxk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gephnqfyy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvxkulval.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkyjhjliv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gkjfjjkyg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gusfqjfid.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gmbjvxeke.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gnqrofunf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/ggrxravdi.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gxesjtvmk.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gbnjlodyb.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gkkzegyat.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gglzctcvh.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gudsiuxjr.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gleisxtuz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gzzfckohb.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gghpqdhkt.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gzrwlabkx.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gfxyzyusm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gdzbjnaay.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gqpgcpogy.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gbcgisgqk.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gojskipxb.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gxzwplgzg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gnsqotork.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdmlempiw.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/guejuqljb.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/ggkjbakhn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gouvhuvtg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gayecpkjr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/ginzobtsw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gkxakpawb.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gzfonfbne.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gtxofyymv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gajpdeelu.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gbvxdvobe.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gandbhpvr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gnkwzpxcy.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gaafngotn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gvnecsgvt.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gmrcrqxhv.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/ggveydnrr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/guljuamri.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gkmjufwwz.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gnzueeogh.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gzzxmcnvq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gcnacvnoo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gwowojqim.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gduvapify.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/grbdxvzen.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gclggxvem.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gtrplnkdf.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gtkmpojuv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gfvluzlgw.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/giqaepced.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gxzmdppif.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gflhxxuxn.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gvvsaditq.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/getcvcvza.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gmmdylywd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/grbtcmnfa.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/girzdktlc.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gclebecef.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gpdqyemtp.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gdstquxor.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gbgwvnzra.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gtkzrbefh.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gjxkenppt.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwpzzgyin.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/geqikzeap.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gdufnsfxa.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/ghsfpwojm.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gcyigllpb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gkbawjwvv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gwbqrotdw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/geyvrgcny.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/grczfgnfr.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gidcudcno.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/ggoevzjqy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gitomebok.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gbxsvvsqs.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/grsaggubi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gxhjbxnvw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gwqhqheyv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gtrbtzgzl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gerkljkdl.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gawmoylqb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gkiwctcsy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/grrysmrgn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gemoiytpc.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gxrzommfn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gqmwpnmmw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gfxmdmmsh.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gvdticloz.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gaixdotrq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/goyzeipsk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gjunryosf.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gvuufxywi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gxhdvnmsy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gofyhaxxs.sHtML


<!-- 参考信息 -->