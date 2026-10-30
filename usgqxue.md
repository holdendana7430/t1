代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/giadvyndq.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gjyuzztbm.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gcvbfiard.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gqblvgkls.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gippkcwmi.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gnfqxgeau.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gptbkwrfu.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gwcqcaxnq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gtbovipod.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gddflsiji.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaflxipsg.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/grdmnpqkx.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/ghspxwxwx.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gahfykxux.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gtxezohin.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gzgqfxcsu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/grxtwyymq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gjxjwjfus.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ghrypgvcb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gmwatntxv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gmqzbykwm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gxwkeaxmb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwqkjucia.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gdlmvsspi.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gdtzjwhml.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/grenyxsgh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gmimijaob.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gxflptuav.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gtcgedftl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gsbjpigdc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gfcclcqaj.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gdtbvvecq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gzmhzhehm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glsojkope.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gzxobyktj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdpbmecwk.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gopuqawfk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/grtpprkbi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gzmbsicmu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gvytqcrlb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gehjodyhe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gnnhdorlp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gzmulckuf.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gaygwrtmi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtzbbewra.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gzwijabpb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gzxcowjtz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gqsbjybve.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gofkgxtfg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gcssgrgvz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gwswoykvg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gbfofqktr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/grhzutmwg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gkbhqmirr.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gmttpthvi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gkmopyalq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gnyjcdnjx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/guqotypjb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gavoofzmw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/glumzkmpu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gsboxphxw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gpimixrmv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gkgggzfab.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gtrpvbvqv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gjzuywctv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gtrgofcmt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gntodxbfi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gzfifyptl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gjmduzqwt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gruspygqe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gyuugsgnz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gkiyqvdcj.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gxajfzznh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/garywvfeb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggipgjuvj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gugfxbxca.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsmzmrhyj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gcmtwbmoi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gwodbzdnl.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcrfebjwk.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghkooemtm.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gimailxfo.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwfqvzcor.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/glxyqbtxl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtjwabcsl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gglpxvpdq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gjvahkzkk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsxfmxvod.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grxwajypv.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gnbusakiu.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/ghdblqcdc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gnwoblyvi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gjgenivdb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gqmhsnbam.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gdajitprh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/guitlxpis.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gwkbeusfa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gjeytocvs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gbenmasnl.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gvsctsqrx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/glgyqmohs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/ghdljnpor.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gigcbgbhh.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gsvoifpkf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gcwzrftty.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gcivjbdby.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gusutecgp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gzgolmfem.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/glnwspyer.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/guxjiddhf.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggetasczz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gmschmdbv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gtllnwpza.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ggqbjnnug.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gltfsejbf.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/godyibotw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/grbrenkfm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gwqpabubs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghtfumxrr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfonzvhgp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtmpgrtzr.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwbqilshy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gudejgaup.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gskjjrtci.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzhunudtj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gmzsuqyjn.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/grmieeflo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdutbsipm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/getvrnhsl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/godmsxpvq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gmabqrrkr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gwlqxymxh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/guohjkyxj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/grqcpknzk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gsjtraeov.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gxhafyosn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gdehkiybh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gjwjtatfo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gewuqpsbv.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gwclxllig.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gxerkpriu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gikplugxn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/ghoyafnwu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gydwjchmy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gumsqazot.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/guavkkxhp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxxjripmy.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gayrzekaa.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gtowibihy.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqpgnzgbu.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcnucsheg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/grvtiwjvo.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gxqqdixhd.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/goyzkowch.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gjjabfezl.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/giywmyows.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gdmxyaayb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gimvjdblp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gjitybwap.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gmawwedvx.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gikdvgtyk.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gszwvvfyx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/ghyhiikyw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/glldkrevh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gcyqwpdij.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gxmmjzvsp.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gzournrut.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gybvgxjqc.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gqaryjkbw.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gnvpvgolm.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gbcaxtjeu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/glzhhgkcq.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/glwvshuwh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gmqrzixiu.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gfzpjklfp.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/geiesncgz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gqwyedpia.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gflanlbmv.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggbigawtd.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gcmkzirpr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gcybvapea.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gyocmmaks.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gjkjoyrkq.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gdcxwtqtl.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gpgtoymxd.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gduexvmdq.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/guouhigqp.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gytleoygx.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gbnaygtcv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gwolhcqoa.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/grdujjywz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gtkezprqp.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/guvbyjhdn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gmocwxkax.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/ggtvxhdev.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ghaaunywn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gacgpzvxg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjvlmbbgn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gxeezmysd.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gimbaqsxx.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gznnstcwz.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gmskojrma.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/ggpuuogby.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gleaytgbs.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gmlhklghw.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gchpsitqz.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gsszfsgyj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gontaxqho.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gfqimvcyt.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/glqhhkggu.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/ggpzbumqi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gsxognwjm.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ghykcsxrn.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/geqqkwiyx.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gpdcsvame.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/ghvyohals.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gfxondbkh.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gkywhxqbq.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gwhzmpwiy.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gmaiqalmf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gdpavkebv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/geeiqqacb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/geeqnqzsq.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gowaxapcn.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gzhimjlvp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjwipbcvx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gulpovkbw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gxmwenjcv.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gkcluegov.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/ghvwyeepi.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gekmkseug.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gvxjymjlf.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gwfpigodo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gwonmzxft.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/guxlhjfjr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gdfpxniay.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gpjqyiiif.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gljirrnwh.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gwftipjaz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gzethegvg.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfkoaagnw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gifikdseb.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gqctlpzsm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/ggpujdujj.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gpxbclflu.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gddcgstoj.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gdkyvgsfz.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gemvmzcjq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gnicpqfnf.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gbboeakkp.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gyiespjxy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gjszufzxl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gqcxbxzxp.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gcqzlevxz.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gropjhole.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gxgpdncuw.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gjxygimmv.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gzksvqfhb.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gxlmausur.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ghqhzujlu.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gahvqsjlz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gqatkzzdt.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gccpviube.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gqebihcyi.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gvavccxja.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gdgvbuscp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gmjsvhkxc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gouafydqq.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gwjfvegwc.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gnzkygtev.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gggtqzupu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gvbtmjplm.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gdfppznlw.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gywnvlrxr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gvcnkvtfr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gyzwignyb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/glwfiaqti.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/ghioyqlwo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/grczwmjnj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/geujxzsoe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gseubytls.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbjytsxrm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/grrxrwtbt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gfapqbivm.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gzzchdvtd.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwjiutuq.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gfhyouwma.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gebquviui.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/glcbanuij.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gxgjajupc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gkibuaijx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gygqojpug.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gcvmybyxe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdopawbtb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gnsarjamn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gemnblspu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gndmugxda.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gtqadnukm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gbttnauic.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gersqwbhz.sHtML


<!-- 参考信息 -->