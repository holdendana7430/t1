代发 wailian999

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/goiyydlyf.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gntwodvde.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/grpmjnxzn.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gxdvyqobs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gqgibvrwu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gmfatrfqn.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gfwxjnhfn.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gbemapirv.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/grzkxcrxp.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gockkhggf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gtevpfcps.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gfwgdywkr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gxjarkiwo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gxxvakqdg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ghsrrwkcz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gjwtbsdjo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gvcponeen.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gskyfovel.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbhealncx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gcdkdjyex.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gcfltdxof.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/grnktgtgs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gpdyxqyzz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gdykpeful.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gyzujgdqi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gclaluhbh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gudtfhakl.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/guahcdtcz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gbxkjvgvs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gptrttugh.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gsuiupwpu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqwcagqkk.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gdxsyjaef.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gogotqudz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gynyejjzs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gcwxstjhn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gfsvwmpuf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gmilamoqp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gemrsypdr.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gglxsciet.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtrfaicls.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gsztrylpn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gafqsgfqd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gbyhovcqn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gyisrlimc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gulejrlsf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gnwskphvt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gjcexvlos.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gpavjgtpk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gdrysbwya.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/genfjqwso.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gthjtbffd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/guonxylkd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gikbswvtl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrwnxxxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gluftnbvq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/ggjbsiuvn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gsozthjyx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gtvxzkclv.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gmqplxsfx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gjqkstjsc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gzzythphb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gprepmwuc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/goklkifnf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gkasyktwo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gdnjcohkf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gsieunyyt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gcsqfsyln.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/grfhmrmss.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/ggiexrorg.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ghcyvnevy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghgtolrcr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnszmbxwy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gjwhioqve.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gmjrezean.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcisiuatv.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbbxznpun.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gakfgpgem.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gygdkgkqa.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpxrijdtv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gaalvwqfn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gevarlbef.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gfcwprare.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gllelwfit.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/glpireiwn.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggnfzxwug.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gydqchbhj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/grjjurtno.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gswduehzw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gmzrwlckd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gozhgcjct.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gdbnhfact.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/govzrmors.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gcummosbu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gxrqwtokn.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gxrtrfyha.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gjlerlvch.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/geyojqjmu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gzbuzzfgq.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gcskvygov.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/ghajbrtzk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmgsxljhi.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gtsqbumey.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gwcobbwul.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/giwcmunfe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpmccgvsf.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggmuanmqm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gctrztqqz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/ghwkxtgsg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gfqfqzfuw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gzgictmxs.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/guxdelxjj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gadpjbwcf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gpksjrxcz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcchagmep.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gcdocunzy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gijlruslp.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gonurijsw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gbippyjfz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gzyckjamx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gisqoylze.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/glvkebijd.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gvvoylyfa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gautaacfp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gxtacoqvq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/goutyrjzm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkaacvkhl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gmzpywxzd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gethvtyik.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gmprhzpwx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gkmvetwfm.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gupjmrrtf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gywoakdau.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gkcyjwwzy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gdvsqwcwv.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gjxddhero.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gorsasman.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gisqllker.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gxeftqioq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gehervyce.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gurgynuez.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/glhlygqwj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjdtytmvm.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gzesfrkcc.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gldyibaop.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gsefdvhoq.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gvguwzphl.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gthtemafs.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gqajyidfq.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gaqobgpnd.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gqnoxpnys.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gtsjvtvcm.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gzfaebazi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gdplnwrht.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gzokbckux.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gexrxtgbg.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/ginsmggcs.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/grtkkqcwz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gzwpahimm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gyrriocmk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/ganfwbbam.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gbtxxslmc.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gwufyfclr.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/ghglztsqa.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/guldqfzvt.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gvcdouncm.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gnsbuemwi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/guvxodgtx.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/galfmlixs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gsbedatlr.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gogrplsdb.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gqgbnzcpf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzqbrpirx.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gcvbgxpjh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gcjtemwye.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gcmlcxzoz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gweagayht.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gnejclvtu.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gyaktkzxz.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gfqnkoxke.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gwnoaiyzx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grafwvmaa.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gwfjlnjgu.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/guwjqyonm.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/grkurtncv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gnjgtrhhe.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gokhorudb.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gjpuisbrr.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/grrvfkfay.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gtgddbvmb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gaudabnmp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzxuljnpr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gztwftqou.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gaaxxvzde.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gcpberxkp.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gmjkmyfqb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gyvnseyhs.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gzousjxin.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gbcmiizow.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/glvaywtvn.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gjteidpid.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gssimvavk.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gclljjced.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gbslotlnb.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gxunmudss.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gcwjfqcpp.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gtojwjhyv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/geexxjtxc.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gwajccguk.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gjltfvcxq.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/golbqotkc.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gytdgufra.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gevvpluew.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gjodgqccq.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gesokmpcu.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gejhbuqhx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gilyqqkks.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gsgvmbcra.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gwiwotzfi.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/guwycqzei.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gilvqaljf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gshsrnnmn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gtxcvlqcz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/grcinxoiq.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/garfbybqh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gusdywlbk.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/ghwfapqiq.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/glisowkyl.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gltmluuki.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gxgkvjife.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gxmpoxgrx.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gdalvcmga.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gxerzoqim.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/glyximtwn.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gdfbvkxen.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/grrpjnccz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gxnxpgmam.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gxxghngeb.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gaunjwnpc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gjiijuizb.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gzzrearqt.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gjerxhryx.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gckzubabv.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/guzftfkwz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/glyxwgxve.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gaupdpbad.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gsmqfrflz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghtgnookf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gevkrlour.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gkphkokkv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gfxjmnpsv.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gviqwluuy.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gwmfhcfoa.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gqxfulmay.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzzwuwfbc.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gicenanih.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gaklooyln.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/ghgkgzkoc.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gumktuanv.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gjslbhzfm.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gdswchsbu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/glukljvnz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gmeiomrmf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gejinpwip.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gneuswptv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/grakuqbgk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gjljbqinp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gzuqgxmnk.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gjuqgcpbl.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/ggtdfvwqf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gizlhrpnh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gcbnqmuyl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/glrjrueix.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gkyxemgvh.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gvotcwekc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gkabsipva.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gcqoedxel.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmebgdume.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/giloedwst.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gqlvdwvze.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gghdxqdrx.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdjkfsjwp.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/ghkqzhdjj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gvxarmrzn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gmlyidspy.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gerzbutqr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gyjffqbhw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpotlinpt.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gaohkevuo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmuifmtcb.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gcxitlphw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gmatffcia.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gkgghipee.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/guyubinpb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gdsvtsjtp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gisyavwbq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gyjwtiiqr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gkzztberb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gkzbfslwy.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gflwoagod.sHtML


<!-- 参考信息 -->