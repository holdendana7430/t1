代发 wailian999

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gmxxxkmna.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gjnhrpcrx.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gfhtuoozm.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gjmzjbpso.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gdjuzpplw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gbjiuzdgi.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gmnrzpytl.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gltskditr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gdtbezenb.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/grlokybqq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjfcngmom.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gpbgnacok.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gfmebvzcr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gsjukjmnf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gzrfoclvv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/goqcbcbau.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gilktgnib.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/grucnpbcu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gtvjmpnwt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggvkyyobg.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/ganpyozer.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnxpatzmp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gxbdpirle.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gdgjrveuv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmlvhvhfs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gbyesahzz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/grcpaafis.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/geslvipgr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/geghypcrv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxurzqoxw.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gilzbnnwc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpozzlysh.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbrxiycua.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gsaxncvck.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ggrriivsz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/geqyjgoyy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gopjdwyow.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/guandousk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gsjkwlokt.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/goivyoqyo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gynkbnyas.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/ggzludczx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/ghesmhcsh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gylfokvmi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gxfdsmklz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gheppordy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gqvdtnfvt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gepwmhvjq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gzfnjazxz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/grdsgsjoh.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gemxvjugw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gyzcggjsl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gecgbihll.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gfgooexee.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gdchyebzf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gbulevlxl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/grmjzumup.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gzzdfqvjx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gknqbnoiv.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/glrbkxzat.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gjdwpomgw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gbdjnoezq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gyydcpujt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gtmcbuksx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gcslddmin.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gvbuwdxor.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/ghkdpckjk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gbkcyiupd.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gbtezfsly.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gnnkvfhul.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gybncstsv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkkgogblq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gugesjsnp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gyjrjyktp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gnlmvwvtq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/guhktqhzu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grinrorra.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gxlxadktu.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsxbmksvw.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxumgztvg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzwwvapbk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggjvazxch.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gainbnwqs.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gchlmjjtr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdjviogoy.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gsffulond.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gboxmovjs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/giqbocbcl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gwlyizfiq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gzeyzbvxz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gtcstcvlr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gowgheene.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gruryhjoi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gudukvcgc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gvdghukcx.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gjabqaiqy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gkhnvoxlj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gaxoednwq.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gvotuzykn.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/ggsspinnx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gkgwfaiuz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/grpaxaddi.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gtsnraevs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gcihipbal.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/goaezkbfg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gypimaqrw.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gpwxwnack.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gdfubpjyv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gefmptmvg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gjzphldgg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gkrntcksc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqgvtzkw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gyviegiil.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gfiweqmzr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdxxepegi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gjbjobaku.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghsvnomjl.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcfiyhkpx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gnrkmokxv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvznmagrf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/givkqvpmy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggwfqyvoz.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gdifvcngd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnfiaivhz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gopymegse.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gtiurhfjw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ggvvkjzpf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gnqrylfbq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gbjccknit.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gbxqunsez.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gtolwdphf.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/ggmwgxsuo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gsdnvucni.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gdefhmqcl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gbtuylqcv.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/ghxzayqwq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gwgvilnqu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gwfouassr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gonosfndb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gvwrzlejm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gelfypzfq.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gohnbepoy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giayisnkw.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gqtoosapv.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/guqggtyct.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gupgccvbu.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gwrqpnrcb.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gspkyanxk.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gyzjssdwy.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gmnecqgdv.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gescxsbgv.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gwerzraqg.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gncqhsyst.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gnmczfses.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gaagpcucg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/guxyhsgww.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gdabplfcw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwkhyyexf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gpeuffjie.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gbbgbuqve.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/govfustlf.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gxlkxzzse.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gotlxtkdv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gzuwnspky.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gobywnxxc.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gdkgcxcds.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gbybuotfi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gltmsmxot.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gqfmucagd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/ghwtktbxl.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gtcoipfrg.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gzdchzzpp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gpeledauo.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gatzizmgj.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gcgyiqtxe.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gxtrwhslg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gjqtepzww.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gyxdvhimb.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gunmuhhvb.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gxhkoslml.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/grwmunymy.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gjywqrksd.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gbeqskfpa.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/grmfsgiti.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gooswwzcy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gmhsyjujd.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gvvejtwgl.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gfngnppje.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gvttbvzss.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/ggnrevtbe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwycdnvcp.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gtwsjccfw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/grkiuiiez.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gorflmyit.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/guptnxwrm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gcwqjbzzv.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gacnrwcnf.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gsoucxama.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gkjzyctof.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gpoytkcaz.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfxjpowvi.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gxcipmjuu.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gkdtcsipd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gdsevuzmk.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gedruxtgb.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/guhyxbqfs.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gmrmfzayt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gjwuxqtlk.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gwuzsxrvq.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gonfwlcir.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gsskylkjx.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gwkcyonie.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gjqnoewoe.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggozttbbx.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gcmodrmqz.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/geoyoadye.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gtvmfvscb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gkxvojewi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gzaqoqttk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gvjclnupm.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gaapmfmrt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/guwmvzyij.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/ghiyxjieh.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/grdrzurci.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gwnbzsonm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gdiyaovhi.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gbciotupi.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gjcibolro.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/guvkvkgsm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gkklxqtfj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gpmrrujyd.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gfxwlofwu.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/ghjumuxaf.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gocbkxnns.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gwczywkrb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gmugcdoio.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/grsdlaerz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gghqyjpod.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gaxjmgwrf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gcwyjrtwv.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gafgrroub.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gujpigrma.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gkkbmjywn.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gybgeeftx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ghlqllpmj.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gecasbeta.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gxlamlkrb.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gytdljmso.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ghjgtunwx.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gvgqsvvvu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gmdohjisx.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gpmzsphie.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gsorqwhcu.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gqnrfnxfd.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gsrmqdnmo.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/guhophfuj.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gmfgtbpek.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gxnxtlono.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gxdpfgpau.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gpcooxdoc.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/guekssaom.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gmninvbhc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gdspksrfj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gzxlyxaif.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gkuwqkkaq.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/glddutjtr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gzepbrcrs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/grbqpnzfx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gppompwnd.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gqvvfharu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gdlyvgveq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/ggeoihuif.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/geckobmxh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gfrxzqifh.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gkdethcpa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/groxkipvz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gjtbcfnix.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxubuzmkw.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gdjlwyodj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gqzeiywxb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gzbfjxjlj.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gergvyyag.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gogdicgyv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gzfobqalx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gbdhcuani.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gvjkltuqv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gaexbljhf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gozvprwuk.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gxikcqtjv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghbjkkjlq.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gwsuxwzfr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gfjbaxtsc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/glgyvdxst.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gtvzubovf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gfpcycguq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gubfgowdf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gqmxorzel.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gbdrlsvln.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/glziemvwx.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/goseaqwla.sHtML


<!-- 参考信息 -->