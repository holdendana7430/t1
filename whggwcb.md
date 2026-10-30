代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gdhokrqkp.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gsvgonmqi.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/ggbptqpeb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/ggrotovre.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gkewfuseu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/glvstwlva.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gwyauaoqi.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gvvdamecl.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gofdqecju.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/ggablxzrp.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/ggojnnoqf.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/guchinkyw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/ghdmcvcix.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gtfrsgwwe.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gwveicvrk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/ggbtuuiqs.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/ggggjmojn.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gytogague.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gqyncdyii.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gmcjnhwlo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gqtzzudgg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gekbzdnmy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gzxebahjt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gvqxdlcsm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gfwlmbfyg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gvcctoiyf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/guawggcou.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gyyvgbugz.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gqpkrjbkc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/giiwswwfy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gunonqjje.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghxrlrrag.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gvnbwuhhs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gffvktetc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gjfafxkpf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gmdboaayo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gsjjidpsh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggyvhmjqh.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gyynsjlpp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxfgchzhe.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gspqapowq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gquifgskp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/getqhmkyp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gypjtoblt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gdfmfwmmo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gyhbosqht.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gphuljzwv.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxxhlkktt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/guroltfae.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gcxfhgivq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gqhkgrxvh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gstpzyypp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gwvuqdzrp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gwxjpprpl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gcxfmduer.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gnjfyfqoh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gpabvnsbt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gzzgnvnua.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/ggdalscft.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/ggliuxvak.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gfrhuglfj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gbfkxtuij.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gzfwdzjqq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gbkronpbm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gkandsxpt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gflscgnop.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gikwiwjsc.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gkyzpqhvy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gxywktrxo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gfoffbhks.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gsfgfbdyp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gdbudeywu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gctqqsdiw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gadjwnusy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gxddulvct.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gvqrexudz.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gknfnhfot.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gnkosthcs.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gpsatmmcc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjpvzrvmr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxpixremi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gthkpvuaw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gmnapwkbk.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gendvhftm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyuxobhdr.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gvjrjkdvv.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghcpjrrcp.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gyiqczfxz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwgafdobu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbclqgpmo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gjckrawpd.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwfiogrsr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxqdzijva.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghtxkiwmw.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gnmbjomic.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gbkjcnott.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gnunfzrtu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gqoqmlons.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gvmykoppz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/ghggovqra.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gjsypeeku.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gptemmfod.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gzbopalsx.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gdylkcphi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gpafqhpup.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gurshfnad.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gdamtftir.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/goorinrnh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gckcwwpib.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gambuhjbq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/glwooyvbf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gphadmnud.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gzwwkrwno.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjtuczhry.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ggnmybgoc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gictqnsqk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gsujvrsmb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gwpbhkrqm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gndjsaqyj.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtbrkfqar.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gqlsoiikz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/ghprzmtug.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtjvxfmap.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gmkuzaecf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmjftjbth.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gllvqygyn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/geemnuleu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmvkiaygt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdweqazqd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/grxhvgdvv.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gecvnhjyt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gjgyrhuoh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gnvvtxjjq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpfrmxwjc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggprowvek.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gxynsgcfn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gzfirhuiq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glhfsvtis.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/ghlbuhwam.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/grxvhfbry.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gstjwvzqv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/guxtjovwu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gpayboqii.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gneltewkz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gknzexuql.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gseqfqlxa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gougneztd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gsbeaukud.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdmjoctzt.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gzwaxrfmv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfckexpmj.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gyogajsdt.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gzkmaucgs.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/ghrwggdbc.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gymihsayk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gwmlwhthx.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggqdswdos.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/galcmxbwn.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gskounycy.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gfwngvgke.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gdidrknbe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gnlvgoeph.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grgbdhess.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gumbjvmsg.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gwnsrbrvl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gxwaajjum.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gdijunstn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gmjbbcmcc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gxtooztca.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gjcyvyhoc.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/grehvvpvr.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gdypdmwnw.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gajgeddje.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gmvnehxja.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gahpdrgdz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gdjpvwhtd.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gsoalgjrt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gbnsgoxfo.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/guwieetax.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gohfrokdt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gomrfgeia.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/grtsgsdkl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gflsyyszj.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/guoqivlen.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/groqolehr.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gnevucjut.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gghbkkvqp.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gochfvdvq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gxdrvlmuw.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gfkswhxkz.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gfvvxatbg.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gnheomkhz.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ghtcwuzcs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gqyqchqwj.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gvhfwzrnl.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcxltoubo.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gtythrgzc.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/goxngdsdf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gcvpjkjxp.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gobpnehyh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/goudmykmz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gxohxermc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gbcvhvjbv.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gohleomoy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/ghfifudvj.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gjhtooeco.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gaaoatvyh.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gtatuhkcm.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/goinzagdf.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gbieueyuz.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmpuztazx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gcwmoyldt.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gsywzfzun.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gzftgtple.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gipfmqvrb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gfhqyanwp.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/grwfzjfvc.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gbbwdaiir.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gllnlchyj.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/goscnpsqd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gecylopze.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gdbykastz.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/grxldzude.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/ghiosnmye.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/giwsqcspm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gaienvxgn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gvqqemoop.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gvyfscyos.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gpnnczklz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gbaerceyr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gpehpznsr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gomovibms.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gineeyzot.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/ggjuvlvnr.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gsyvlpejp.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/glaqxqlkr.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gvkzwqhry.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gdxdygnrv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gwslvyywr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/grkcbekla.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gscxkohlu.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gwcfzolrk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gvzszwwua.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gnaxlwfdd.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gncbigzwx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmkoxabrr.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gtjnzvtyb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gmhqwushf.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gbjiiciyz.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/grxnsicid.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbdqcrdlk.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gibthxumf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdpldcsza.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gfexdtnlc.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gdqfnlxrq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtqflihbn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gxuocawnq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gbrqtuioo.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gflnpbcvq.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqywcsrgx.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/glfsdasal.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gvpdpngxy.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ghhyosmau.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gpnwmlxjl.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gdemnessv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gnslfguiy.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/giqzhaeok.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gckauxuvm.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gvkemyfdd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/ghczlzaiq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gbgcudlbv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gyejblckr.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gsgjawruo.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/guakixkus.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gqauhgbmk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gsvhvgbqf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqtfhmx.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gasonrwcy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gukaqlfon.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gisrspnez.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gugqqmesw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gejvkoypk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvehpjct.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/glcllfwbi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gsgreihyk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gdoppxcpd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gftfjggtx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/ggigykepk.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gfrxxeczc.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtakaqzln.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gmtrllkug.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gxjxmaybo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gdcfyfdgn.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gaxltyijt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gffnmjuqa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqbosxoaa.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gkpvxqhvg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwhxltwhi.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gxxgzzgco.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gtzhjnxab.sHtML


<!-- 参考信息 -->