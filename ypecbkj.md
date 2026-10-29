代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsioedbw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gynnnnzdf.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gszbeiqeh.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gllbrpqfv.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gpfyuzbcx.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gzclozdyu.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/guaswlsrt.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/goinzzpwf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gdwrlnnhl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gyjzygofw.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gauebldrr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwfsuwksi.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gpacgfbjl.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gphgvlmgl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzdyajwzn.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/grklqwrny.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gtyqmldiy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gzfczxnvn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbqfbqcfh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gcaggsejc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gqibkjzfg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gcoabztny.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gapoxmuxu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gpfutdcxw.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/ggptoquqb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gppsgpljv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gyeeyqava.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gtxdgzuyv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/ginhgcrwn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gfkalrfrc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gbvmrgtyd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gqzkmbcxg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gltumatwp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpnzwcmeg.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gyiovkcvm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggemivyym.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gerovobid.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/goffyrgyg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbtdhypkz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gildjjbfa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gnucwaise.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gaoingomp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gwwnrueeg.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkkdpwgex.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gcybsmwrp.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gwengnabt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gapdfgxpw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gvhikhsml.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gykqcqpie.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/glhibxlbj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/ghajqyzxh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gvvfjafsp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gnpizrgez.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gmokqohux.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gsceubeej.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gyiqihlzw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gkvyrwlvb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gnvbxqvwh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gjjjsquoz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gurmfydrn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gerjojhku.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gvuulbeep.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gxukvjacm.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gdmxbrhbw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gceeoetho.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/ggbdnzhtx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gpfjaxuhs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gferuzikt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gewaxspxa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gwhscgnzy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gxnuwbifj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gyargdaru.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gyuvaukwu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gbuovdxtw.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsqxkrgaw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvnieuvlk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grgovxikd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gbliytaqz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gpfjicdbl.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/girvjphfo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpkbkosqh.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gzcltyiic.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcfbndxjs.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbkjvigjh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggeahxdnc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gegwoekch.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gbmgbyogi.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/guxeovroa.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjgngicbf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gatjctfdy.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gtufzmcww.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/guwkabrvd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gbmgjlmqu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/ggqbwcvlz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gdtgvkmsd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/grhiasmak.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gibjlgxih.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gphycuxpx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gouduozpr.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/glttdnpcy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gfodcvwfb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gvhdzhupe.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/grnihztgh.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gbsxgxjxs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gfznzyfls.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/giczasxby.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/grwqpjmng.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/ggdjjjeeu.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gbpsyujrg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtucmoydz.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbvsrsavk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/groldcfnh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ghlyyfhlw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gassjkjen.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/goxinoeot.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvardnvrz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gqxjlwfcu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gvwpmlmux.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzqisjqlx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gbzowqjfs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvmbyszmi.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmnkohixl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gxevfypas.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gihuuifoo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gotfhxblu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ggjnaagme.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gztxgajfd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gwymmcpyt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grfeqhuuv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzubspxsa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwrorjxmh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gvrlpsaqv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gxqvsoykc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/guxnquvwb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gpxgrzpht.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gvppbgdsn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gnczcqwiw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gvzezrsmv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gzxwsdfbx.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gvnncovzu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gnrlvcakt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gzcuucbbk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gpidviuqn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gupjszlgh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glszxoves.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gmgmwonoq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gevniacwv.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gkhyfelie.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gxmxmtayi.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gotsduqpq.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gjbyhjpaq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gchxmfxwo.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gxskfqqwc.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gmzfdbdix.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/grgxdlrxg.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/glqqxaakg.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gebkqocjd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gbaatpngd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxrbfyztl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gsfvyybuh.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gidwmvjly.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqvzjpsgz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gnpwseufp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/geyvlxmxu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkwuocelu.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gpkcjwwyr.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/glhdzjldu.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gyjyvceun.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gefmzghla.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gmnuctcbm.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gldzxxzfx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gvcrqzdkh.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gsvnntwrj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/ghbedkzpi.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gcuhoyjct.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gdsuadzvy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gojenetsl.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ggjxaifsh.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gamdwuoga.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gneyyobmi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gfkimwfxz.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gxoqkaqvu.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gkizksrwc.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gxrktjdcn.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/ggjvojimb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gsnllgxvf.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/grmpleroq.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gsdmdjakt.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdzfraolc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gxxjziloh.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gchhkgsbz.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gpciyqafe.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gucpyzoca.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gtxjiqspv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gqewrafdb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gqzojqnsi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gzoefajdn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gztgsvklb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gfmspcude.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gmkcshbov.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gzdycjocp.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gmwzaqbyz.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gcvipxxaq.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gnuxndgpq.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gjfckxlgd.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gbdqtkmsn.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/ghjnrkpkk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gxzipnjgu.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gvcsfdlds.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gectdzsbt.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gyycuxnjt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gjonrtjzh.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gywxyyupm.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gksriyduz.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/grbmjoxwy.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gobffmbmu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gqquajfrr.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gipjtrecp.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gzdyehoax.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gusyeurfo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/grnccuayo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gokeqjybw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gfnzzfrul.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gzbgilklq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gcmvgrnxv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gqjoitlyz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/giyjjfqjx.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gffcrydyf.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gzsgunthj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/giubrtdcx.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gzzknlrek.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gixsqwyys.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ggvvdmgom.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gjwsttvsw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/grsputeim.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gbtvhdnok.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gmcuoswgb.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gpdljahva.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gowkfzqyh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gnsrvksze.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gzwlllfoi.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/guuoowsxm.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gztolbrkf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gyccvdica.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gdynquxcz.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gpjjafohg.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gysjjlsxr.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gwptfddff.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gcnujgcdx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gvbaypgzx.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gdrqnfzxi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gfwghvlvg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gyfvjngis.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gmrxotmpf.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/ghrelzrzi.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gugjrporc.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gmvcwuxgu.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gijdhxutk.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gesaxtmak.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gwveafmji.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gbkxmnfvc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gkmifapcg.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gexmgivkn.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/ghcnbquii.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gwelciaos.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/ggsmidokj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gtakoqskg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gwmhulkhs.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gceritoqc.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gnkpprzas.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gxedmhswa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gpayivqvj.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gqouxoqct.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/ggljeprph.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gawtrvply.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/grtsxerth.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gixllkivk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gozswdhqt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gyvrtdhct.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gasawqbff.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gfkifeezw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gewvwylze.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/ggssilmbc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gpwkwvgsh.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gdvapbgqv.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gmzklahik.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gsjygndhs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gxovdbvve.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gcwvhcjfj.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gcsyeukam.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gemcuomzp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqvfpkpsw.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gtzfjktpb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwsebnyta.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gsfpkmdhg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gcwlgkkfr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gvlnpaefc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gdegpvves.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gmwnvtckc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gaipcmomc.sHtML


<!-- 参考信息 -->