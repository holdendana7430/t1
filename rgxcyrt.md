代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gtlkbnemk.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gdirgiijt.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gkbrbrtex.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjkhrzsjs.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gtquqdaht.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gsccgjufe.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gfkqztwau.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gaolwxmwn.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gomarhytu.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gwosgrnre.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gsyzcbqjd.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gdywblski.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gkxnyovyb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gdennthzj.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/glaigsirn.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gupzgjwij.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gtwacppup.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gooyayixy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/ggwdzkkxf.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gnpneahtj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gooycemaq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gnbyybzgx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gldhnxwto.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gmmeugzsh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gyvfwfwdx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gfaxxnerd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/geryrxoms.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ghstpwmqc.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gbtjrziuo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gwhooycza.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gtphktxnn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gczpmccau.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gqipjfhoo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gkwqhbzij.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/guimqdvfr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gohihqcvu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gwtdhcrow.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnmoklawq.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gqetaahev.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxkzatpnp.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/glpzbzqqc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gvtqdzrzb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmietwfmc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gbhgcckgn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gjdmcuiwy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gchlhmwyb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gryirkxcf.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzkbokweb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gijfjqahj.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gsjqgyfqo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/ghyqlymlw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gqrowxiod.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/ggykpewxn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/golbvqqwb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/godjloieq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gqkydxjsa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gtaxffgkx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gimkfflan.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/glglhdpak.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gamlnxeii.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gtccocccd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gebudccvk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gdimqvqhc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/glshzadik.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gdtzuereu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/grviatlpz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gwffvisih.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gtnzarfxb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gxllxmmwx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gwrjauvfu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gymlkvlkn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gzertdcal.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/ghosccjin.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gjjamqhdt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gxwtxddsj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/ggmafporv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gzlxicdmk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gfifewaot.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcljxmhyq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcrchwspt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxshxwlem.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/geiqlqoxm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/glxnhnuqk.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsjvtifet.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdaqxtkyt.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/giiiykitv.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcorxagee.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gqrzisias.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gazrfhtgk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcykbabof.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gpbzgcnlk.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gczgabqux.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdgifvjdw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gasckotfz.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gowbxwkxe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gzogvqbxp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gvaqbfcwy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gydqqdyqk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gklepfrfd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gezvntfwo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gxhnsujmw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gytnpzrbs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/giphmswyl.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gykozdzwb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gqsndkwey.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gqbeqezqd.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gaviizlhu.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gknvodbwx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gqouynhtd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gcpxypmcx.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gdumowuds.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gwmwmjzfb.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gbzfewvkg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvaywixav.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gnmqnksnl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gsrqbfyyv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gjrkdmpny.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gpwmtbcrd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gjqiempju.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/givgqyyzg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gawfbixgb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gueymbgcc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gylboeraw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvuiwnedh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkvxxagbd.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkazldcpx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gcbgheolg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdhjnzzij.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gmkfvphvv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfewqcncn.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gqtwylsql.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghupotple.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjksyehht.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gpkdnmqhx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gxxmbnvxj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gzhxjgnxb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gwcvuylxf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdniomukk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmyopfbr.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/ghuoqjuam.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gjjybzcpe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gzzkptcux.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gkaelaiyo.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gestzzhsy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/ghoanrruz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gnfoatrqt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gkgvfbbjd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gzsarrnzk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxzhejelz.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gsuazpqfz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaqqhbhvv.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gamavmwcv.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gboqrijjy.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/geuakahsd.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gszxkenab.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gphcaoirs.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gvouanplp.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/goswnblxl.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/ghtwzfrdv.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnjvsfhil.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/guvhkpkaq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/ghhsfbcxj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gnbwlssqv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gtjhgzrxo.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/glyvzifxp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwnhwkdkp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/ggzsmdzqs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gdwcbnhsh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gdquafgqk.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gpjvkauqm.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gxvbtdbxq.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gkndduukr.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/grpcmgmbt.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/guywnolvu.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gmnwtoijt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gieegwqkg.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gbrgykrvg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gjldsuvqg.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gkmbcpyno.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gsrperljv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gcsfrzicf.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gdivagfdx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gosioojhl.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gauqqwiwz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/getecwctc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/guvsgfgck.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gwesoydsk.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gtfjiysgj.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gknawtakv.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gipudgvmi.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzwwbhehc.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gqevbxdxe.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/geigejmru.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gvvzzwief.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/grshcigju.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gnppbabvm.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gnizwxiov.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gwuhfrhbv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gnrxwatot.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gdaggbovp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gpoqfkgnx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ggptpvhnj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gqylmvnib.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gmslxcbwz.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gjqccutfj.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gtobnroqv.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gvnxdqjlb.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gboruskvy.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/geoxugbhg.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gngnhijqj.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gwnhrcndg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gvhkhkgmg.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/grldgylls.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gplmtfpfp.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gyyvzmhbe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gpefdeiph.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gfaguzicz.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gtbbloynj.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gxgpvdqog.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gustuwyop.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gxbjnyeev.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gusnwwvwe.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gmexttrvy.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gkhghftav.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/ggkgztznx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gfupyhobi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gedmitlgl.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gqdbvggoi.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gvornmdud.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/ganojvoob.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gjtyphcif.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gifzyogpp.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/grqlmqlhk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gsucltbzk.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ghwjgwtwz.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gnpimzyvu.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gahwpuxee.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gvmbydnev.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gmuomxrsw.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/glxbsmkfw.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gfjwurlfp.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/ggselltxo.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gpqdatnxs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gnzxjxhrp.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gowstneki.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwanfytec.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gervmxlej.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/goluchzob.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gpygalucf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gbmoryubk.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjglyttur.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gtnlyybgr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gzunvyszy.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grnkhdkaq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/goqufokdl.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gifkrpsls.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gveedmyew.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gmgvaeaxu.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/ggqocwbvv.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmuvnegzr.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/glfgqrdph.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gxscqrpfh.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/ggqkrobdp.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gfmtddxkn.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gbqpfmztn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gihiqnelu.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gejaynxfa.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gxoqifgsz.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gqzxkpubj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/grgqowklv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gjqqczepo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gzagiadbr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gtnwkeasv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gxsfhhlcn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gotxqdhqt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/ghhzbqfre.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/grmnsurmi.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gyqazztgq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gmqfahbyd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gwcrumgey.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gaufvdzdf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gcaeqyhvm.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gzyrvnimt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gwqzucbta.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gonhjoxmc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gggcqvhnj.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gvwkhbtut.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/ghtkxnwij.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gjfeeeflx.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gcpnkqhbb.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/ghijulpbx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gvlsmsyos.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gbxxmonqq.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gpctrkbpg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gvjsniqkp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbyogjock.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/giuzfrwpm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxffoudtw.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gbkdhmjws.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gccwrfwjo.sHtML


<!-- 参考信息 -->