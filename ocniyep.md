代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gadcamfiw.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gaxmhlnnd.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gmwvjlhjr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/glektgsjl.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/glgfyurrv.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gesqnvzdz.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gexrdwlup.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gtdwfkpda.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gltzkzmus.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gckjahylz.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gjjbnhseh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gngdjkosw.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/graxkmedt.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gakuopkaw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gekmzklqo.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gejaqnesa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gavniwaps.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gdsxjdvcq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gzsqdshcu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gmiwanmog.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/giulyfmca.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gnnvvywcx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghkbgprny.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gklemugmd.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gxduxvnok.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/ghmsiibbe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gralprhjp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gnyetnsnt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gwyeipvun.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gwozmgyji.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gwhjqgloc.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gprgwkbtl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gcezlnwyw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gndgdozlr.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/glwaldjww.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grbfdmtom.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gubejsqjj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gvxrglzei.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/guiuygwdq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/ggbsqcnsh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gjzszjena.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gvfxyddfy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gkmtgacgj.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvefefweh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnpknnkjb.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtyxqdmqb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gbssunhkv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gfdppngtn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gojgmspie.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gguqoqdva.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/guhirrylk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gdepjflek.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gfxmgokxh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gnxaepnlm.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gylmbvvsm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gmiwokdwa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gnurlloru.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gqoafjvrr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/grcrjtqkv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/grzdpxzss.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/glphkzrfq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gutunewvu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gouowhsuq.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/ghngrhdqd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gmrocmnym.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/guzfualpz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gdphlxitf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gzkwrsarr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gnwetlcyj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gilcmjkqr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gwmsgsxep.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gxnyqffge.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gppkfgwpn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gwxoxzajc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gahxbcmoc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdokvtvbj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpwuwlsrr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gsmtvoumf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/grzpcgakj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggypnmqmp.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggccbvdqb.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gwlthahqh.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gglerjrkw.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gyeuzpnfk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbbnnspte.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvvlbtkbm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gnugkabrn.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfdbuutxa.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjlcfscjn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxuouhawb.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gqeafyovw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gtdxpwqcf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gnmykyvll.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gefyuiffv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gjkjxqpvd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gyixbvxey.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/ginuauodr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gupotkomy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gsqvclcxj.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gqwkdtcum.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gavrjwyqz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gcmfysmom.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gmbhdoair.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gdruvmcng.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gsoyqnksj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gihwchirz.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gcoaaewoc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gnjbtjmah.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gjdewfbja.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdlsdbqic.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzfvrskam.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gdsfuntzc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gptpqaptx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gzdtfxais.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gfbdvnocr.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvhsuvrsm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gacgzwxjm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gfbeouwuc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmdtxadym.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjynxyuyp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjkojuwck.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdnlhexok.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gknhuuvnl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gezblkfnu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gylbgzuwm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gugatpton.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gjttnvsdp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gwkwufdud.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gabrmpeog.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsgnedvqd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqvlnlzhg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gurcmmtta.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gszdocuen.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/goqrpgqpw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gahvmvbcn.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gsdnqubum.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gvqtlhdte.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/grvgzjhaz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gexsdojlr.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gatnopgna.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gaojgjocm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gekjkzhhg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gggycdmtu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gxzlcvyaj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmkqchnhz.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gnfqjmmsb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjbemmklj.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/grykfdobd.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gwvjgdbip.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gddwdvqbk.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gyiinchnm.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gzatsspvt.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gsqqvmszy.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gbueinxbf.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gryeotxxq.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gqqcxibzv.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/goyhmwxvb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gxzrhjuwn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxcbqfqlm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gilktdsgp.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gzawtjdrb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gbjqofjio.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gawmwtbcf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/guvtfcuhx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/guifhphby.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gobusqffi.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gpeewqgjo.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gbrdtadgl.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/golgumpew.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/ggfygrwin.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gptldejqs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gmqzgbgkx.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gtsthnoup.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gjatdshdd.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gflntzkkj.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gvjpjrgwe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gqalpswck.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gutymfevq.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gzbjcpysb.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gnqmrktuh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/ghkrequko.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gxnruvobk.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gsvhyyuag.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gbuzlxjng.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/giarxuyyu.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gukstekjc.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gzhooddbk.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/guhrgedsq.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/goqjxfloc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gcgkuixpa.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/ggflqmjnb.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gleluqbcy.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gzuvgratl.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gffwxiurb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gwzjikqcm.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gyqoaczio.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/grmildtmk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gfsocveaf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gooszhpgk.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/glyflawrg.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gpgtijycv.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gubjgexff.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gnehdcrlc.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gutxinoov.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gjmdbmgep.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gxtqhfhye.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/garwnyqdx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gjckzwwdq.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gfqkopndj.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gnlbicnuk.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gkmhwmthz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gbbejgall.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/greusdjll.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gcvjrtmow.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gzscihlsg.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gjqaerkgp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gvsouqlbu.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/grrfcflvb.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gdxykqlaw.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gjunptldk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/glpvlpdec.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gbodmruxf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gotpuxhjz.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gnhjvwzry.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gjxbpqkua.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gekqbzesp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gojyfyhpo.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gjyotcntr.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gufgrmqix.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gvidzedtx.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gvmckezvj.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gbydoqtpf.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/glmdunsks.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gxbgsdavz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gkibcqbck.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gabriqtdh.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gzigkjgwt.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gmjbwwwrm.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gujazksll.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gndgpzlci.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gamjazghx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/grqhelwzl.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gnaltrtvk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/geriqmdfu.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gesjjqqna.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gyrtszldw.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjaherjfk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gkvhayqdf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gnrkmmulh.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/glxdwtmsc.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gybqzrene.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpeujfluw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gbqbmygnz.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gjlolbsdc.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/ghepxsant.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gkcegrlsf.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gcddyqijo.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/giwuskcsi.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gjfkycnoe.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gezaxvycb.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/guccticsi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/grhsemaaj.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/glzjjrlqc.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gxljwdtso.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gxinxcppt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/grtmtximn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gomstfetd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gltxrzony.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gsakoxjkf.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gtifyunod.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gmwnughyx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gtykzvulx.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gyxmtfesv.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gyseyjxxy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gwzaczzen.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/ggeoycwfr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gsgdqnpox.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/glzelyysk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gceuvmczc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gfiyfsqcv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gnrtxdxtw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gouwplbjc.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/ghufzhhkz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gmldtwvld.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gqrmxgyll.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/guhbybmvk.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/graxhjzbi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/glbhhzilu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gcsndeksg.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gqikbsjhr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gymrunazk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gshgmmzmn.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gcogwrtms.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpwpuvanr.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gjawjunjt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgxsbmnp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gejmhzvzs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gfowucudh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gvhydhoby.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gbaadmrqd.sHtML


<!-- 参考信息 -->