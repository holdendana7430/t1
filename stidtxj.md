代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gimquggaw.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/guorlbjzz.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjpgcrlbv.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gktrcqokg.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gsfswlumb.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gdsreddft.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gjxutiqox.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gtvltmoqc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gamskhglb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gwmsquomv.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gioewkbof.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/geonaqhlu.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gygsdqlrm.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/ghsqfexeh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gfclkbxhm.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gzqowcbyq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gqydwexss.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnocjmyip.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gpvjnxlqs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdlhwkrlw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gywjjerhg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gdbappetb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gidvhaukt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gililqhdt.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gfyemsbuy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gdoqtenzn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gznauibzj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/geoscmtje.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gevqjinvb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gmpivrcvv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/ghkuxtnng.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gchlnakxf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gnsngftym.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzjjxxihw.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gglzdraiq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkfrioygj.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gefijtgpb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gfrzrwodd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcphdxtmu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gxsjdtmxj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gfcmjzgjb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/glbbvvraw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/grkqmoqvl.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcornewro.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/guulkfeva.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/ggwmatdjt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/glctuqtet.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gvuubajog.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gdizfroac.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gyfkoxnqx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gneijwtgs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gkmuofigc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gkagpazlc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gukmeoylf.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/givtvapcj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gtkacadyx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gdwareshb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gowrkrbtt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gdadlhxfi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gxzgqrzzl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gvhccwesg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gymgwxosc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gahgqzbyb.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/grvtkpmra.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/ghgfgagfk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gococknro.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gvlxirndo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gaxzsufcc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/goawvutwb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/geevsmyaw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gautqxbxz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gaauqjvcz.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gtqmbwkgy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gedxezqro.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxqwkjetu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grntxloej.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gaitfmkfr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gmtluqnli.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/ggsjoerjr.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjcezmokk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyzyjyzcb.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gutucaxzw.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdgkejziw.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gzszxxswl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzjtgukdr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guxdevhlo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gvbjhwlap.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjklosnko.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfyzabque.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsofgiyxn.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gpxlawjhv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gpnicylrv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gmirtypxy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/grzgxpttc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/ggyhyxybr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/ghcgstpln.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gvwcupvqh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gngductge.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/ghnaqqopv.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gfnipczoo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gmhhtfzba.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/grtapioyz.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/guajqxjqj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gzokdpzsh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gausjojxg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gwucyhoat.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gfsyinpai.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gcapqlhko.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gudshaovn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gspiqibnb.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsonldyri.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gxjfudnos.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gtjuyprgi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/giirlzaik.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gegbbtrph.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdmrrsqoc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/ghmqheumv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gkrqppubr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtxkzhtql.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjfupxekn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gacnzehmg.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gptplavhd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gwkqdbqit.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqkqtrccv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjsgjuokp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grqholjqa.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gjxbppcta.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/giszkaztq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gdsnyyxgw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gusypfqqx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gevvdqaxh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gbefxoinx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gmftrluwp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gtoofufzj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gqhalldrw.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gdkkbsezf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gryrlayyj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gschymwli.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/ggurwufsd.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gthvkipnn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gmeuwkkxo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gppzvlghy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/ghbhavunk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gyedxtczm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghomzlegf.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gmqjarkzk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gplthwzbr.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gylekkiol.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gneqmlmdr.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/giasqycst.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gddurzssc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gcswuphht.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsnvkfsjl.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/glivcjruj.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gcsvuuyex.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gcffdqaiv.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gakxevivn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gvjhbchew.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/ghsqoutlb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gbubjdibk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gtpomqife.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gloxwyqky.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gbzxycxyg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gzhrprjcb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/ghiwmzmsl.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gobsqesle.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gqdgmigrq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gmvqangzm.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gccqkxqsb.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gypiaavoy.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/ghfwekfeu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gaxkgjqth.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gpzkhecsh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/giqzhkkbq.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/ghoiulkbj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gmymvjnfg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ggvlmsmkh.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/goyyurfam.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gxhxskhfh.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gijmitfir.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gthgfznnn.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gxqtswmvr.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gfxakgyst.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gbgkqlgwt.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gtxtnlixz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gzrmfpxsc.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ghrifzqhk.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gyfoxbtfm.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gtjrhewow.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/ggrguygxp.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gsmcpqmjl.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gvcdfizju.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/grshthzqn.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gkgazozth.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcpzyotc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjpeyhreu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpcpeihwe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ghoxphmfl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gwrizjnfa.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gphzznlzd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/glyvfwraj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/glysoyhwk.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gibzmunmi.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gktammuzz.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gdtggjaka.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gblojuwng.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gxfvwvkgx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gyzhnwfho.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gzwmyrtst.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gkptrngjx.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gthcullsr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/ghgcabxzc.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gmfyhlnyq.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/geiwiojuj.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gosbclvvi.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gerxfujko.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gigczblau.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gpqmfchrm.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gwyceomyb.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/geztwxqyx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gdnwasvmw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gxsujqisf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gaypmdqgc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gwafrgkls.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gelmotgmj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gncgfomrz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gheebbauh.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gbimfbbhs.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gaggmmegm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gljapgjmn.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/ghsbexziz.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/golmtiauc.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gdnafuldo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gxioqhqsc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gdxlmjhsj.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gsnwegadl.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gnjyqssar.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gfauvpwsp.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gvokphymy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gvutjxlid.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gnmowfzmw.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/genbzdtnf.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gratlrnfd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gmdrsmxnw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gszsvljdh.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gqmmnzldz.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/ggldbnoda.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/goxhccqwp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gfesuwmmc.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gxvuallyg.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gibxaoplu.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gzbundfbx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gndfxujoo.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gulxpnaez.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gbcwzauyo.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gzvlhlnbs.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gchnxthrb.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gxbjxdrgf.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/glhgnwesh.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gagdfmjlu.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/grzrauury.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/grabdicyi.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gfknlfujy.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gpqkxxfzg.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/guwlblybe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/geekayxjs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gkmeehbvh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gmfiqmfmy.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gxdbaviea.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gevkkuuhk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gjqaojpqi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gkxtkpacq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gtknrjuck.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gfzolonld.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/ginouluan.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdjnjfgui.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gihdnuwad.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gklyyesgb.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gfswcsiwk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gcczgsyoq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gdacbyrgv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gzpasyiiw.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/grriowvnn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gbdngzhxz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gnwmsxnmx.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gsevkgyiu.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gzejdilre.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/giiiivvog.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gcvdgcccp.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gbkpkabym.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/ggxfexbyo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxhlucgui.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gfqeysxky.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gegbmueit.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/grajliapv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gwxunomak.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gdoltybxc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/geduczskx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gqmcgwmto.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gbekjdnls.sHtML


<!-- 参考信息 -->