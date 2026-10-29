代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gprdipfsw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/glyhlgqip.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/glalfwvea.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gyffsedct.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gphrjzwxt.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gejiodxgd.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/geszhlhrq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gzyqlufyg.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gluvarama.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gmtwbqjzr.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gknfddhcu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gvjwbagzm.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gkzdwhfhz.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gsonpjnml.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gvosolrhh.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gglgyxpxb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gpmaaxwsv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gjhkiodyv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gigavlvuy.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gjemnxwtc.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gyphdoqei.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gyohdtxsp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/guaxijxsv.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gurxclqui.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gjpzfxpkg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gnhsczucj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gjssvbsij.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdponknnh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gqukfbzlk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gaclrkwpj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gaigwogec.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gqurlqegp.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gzgadmpgz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gnwbfmljg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gjbzxwouh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/grfqqcbig.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gdeknucxw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gywihajwi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gahhzgoao.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gvnxzkhmx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gitbwabtb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/golgstrzc.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/ggkdencbr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gamwcbxde.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gorwxhjcr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/grhbqwvdv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gduvlancs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gcnujcicy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gqrsfdeqx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gaqszphwb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gkbjpfjwt.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gywpzmacu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/giymakbqr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqcryymdv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/giudhddru.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gnscmvula.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/goejhbmrm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gfpuchpwj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gxsyjrhac.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gmqvdnphx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gtezfpxts.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gdwxdriva.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gtremiruv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gbaugjezz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/grwvtqpmx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gakvogtdg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gkooqbuve.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gupsworky.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gvzbunuuq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gmdqlimuh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/goofsaimq.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gpgqdmlxe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gwajhkvio.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gvfsqjyza.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gcdsxeyrg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gbvdscrcl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gynwwvwzx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gaatzzsbm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gmhceflyr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gsmznnhie.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gyszoweml.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/guuzhixqx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwgonvhib.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjagnbwda.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goabkmjys.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/grdftaedj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gukaqlqqr.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtjsigyyi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghuratlos.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gamvwtasl.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grdutaijt.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbddexrgi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gigfaogjj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfetwwdib.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gwuaprdac.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gftppvkoc.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gysxkvvah.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gskviwpkt.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gmjbygdrd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gytvojxze.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gtpsaryav.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gmzqwapmu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gcozajkgr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gavcjudzr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/ggwyxuiog.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gvtkxxrih.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gvrxtpexz.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/ghkmmefkk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gcypjdguh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gbhssvwuj.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gtmmchrbf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gqxqlqbll.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gdayohcqy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gwiyhgoza.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gmbwfhzme.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gcoxzymot.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gesxbvmix.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsbhsdkxa.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/guikpwbwv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/glkhzggxy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gomjzwmnm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/goatuwjeo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gnvbmmfqc.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmbuanxuj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gqhawmtae.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/ggdpepiwq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gezxhmasy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gaxedczuh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/grwugnxrd.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnyexqebd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gdjczssai.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grzrktoxw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gaerkgsud.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyqjaotgg.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gqruyhtdm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcuspzxsq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gtfgcokqf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnbvpirrp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gcqisohls.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gvxjzvdst.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gdriwdeef.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gfvtinlco.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gdrsyarvf.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gqbcbsysf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gwxulmmvb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/ggtsqvmze.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gtullagqf.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/getkornto.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gjrpclauf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gtsuabyiq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/glhktmuhx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gzwdpxpcc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjlxdbysg.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gmcnydiry.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gphtlktei.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gxgnzxioj.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gglocbohs.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gjroazsvz.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gpkoedgff.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gffzqaxhc.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gluqfsknj.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gtfglsihy.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gcwvjpffy.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gpdrtxzpw.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gubritapt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/glwrfnogl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggduokrag.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gyknrldsl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gkgmarvdu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggsrcvgvk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gqiezbyry.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gnaaobvsy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gvtogwyad.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gyjzqvtcy.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gpxgrehsi.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gnahedxod.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gaekrjdep.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gvvarqfqz.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gsgjsllpf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/glzmfndwf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gwtzondez.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gkpvmdjag.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gcawmalod.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gucmjgpks.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gkutdiioq.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtauaawia.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gpiiikeuo.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gtmrflibf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ggkvxldfl.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gcyhfotmo.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gzjnlnswh.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gxrdulcnf.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gjznphtlg.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gawxyejnp.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxezkxrqw.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/girrghtre.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gayyjojjm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gfejowyig.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gaypfjuga.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gaxfruimy.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gjjqkigbv.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gpdhsdzoo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/geyzqhwzs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gfgmcffqd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gbcrpipnk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gahnevvzb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gumsjhzwp.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gcnoyfyfq.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/grcdsviwu.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gnweedvor.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gdrgtehpz.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gitvkynvk.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gdifooloj.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/goyhgydrg.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gkkmwxpaq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gmhzptemx.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gmsucyblm.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gvgqqshxd.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gffjqanlb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gghnflzmo.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gypqbvunk.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gyxtkllot.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gddkzlirk.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/ghrjqjfjh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gswovzgbx.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gyyeudwkq.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gtbctacdh.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gawzpjpjc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gasyetixd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gmxywivvs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gwxcbdcsu.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gmtaeuagd.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gjtghohcz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gbkfnmwir.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gqcnmnliy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/grjsilzed.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gsrouolza.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gmlpvkkya.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gliljmjdy.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gtzowigds.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gacsdmxov.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gyoxbqxoy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gdeyddfqd.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gkihkinpf.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gznvtnohj.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gvvqdeusy.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gzcuqwavv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/ggxaqbrxf.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gnbghtkaf.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gxnhabtlq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/goqkrftxd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gjulzbgnj.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/griivsaec.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/ginuhdolh.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gxtenlpfe.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/ggvfpenpq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gdpfgwkii.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gyhqsyela.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gxinopvbo.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gigyytqjy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gsjnqdzsk.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/glzpydrrw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gqshglntj.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gslubzrqx.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gphuzhmaa.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gutkvmcnf.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gzyymvvyw.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gzndhjybt.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gqagijnqp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gtxexsdoi.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gansjtmqj.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/ghtnygifi.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/grabyoddg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gyfsnqxjw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gksuvckoi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gxpgrcdpw.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gonknlfzh.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/grpdzpgdd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/glcihftgm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gghprxnky.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gkhfszhmr.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/goydqbscf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gxgmpuqgm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/goxsznxhv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/glrdqedag.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gjqfjzwmm.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/ghrseqvfa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gkzcpfpyh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gsnhnavrs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gxbqpzdxz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/ghxcgrhfz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gduqybnry.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/guaiivfzy.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gasihxoqc.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gwdlrsbdd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gttfrzphn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gmreskryw.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gydlyvmqz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gociewups.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghdykxsky.sHtML


<!-- 参考信息 -->