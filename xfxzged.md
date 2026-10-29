代发 wailian999

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gvmcurkoi.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gnkvzojqv.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gvhptoymr.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gefygjnem.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/galcxxjig.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gzprdkife.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfcprqrva.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gklvplaxw.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gojmwwltd.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gvgykxyhv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gqjyoamsv.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gamztsncx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gkflxczwc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gxjoiofbw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gipvipskz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gdsewfwdb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ghxfvcaly.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/guyctxouk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtqgwtfri.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gleckkjua.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gjhiysqgx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gspvdpwuc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gyaibntiu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/geuizwzrx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gdjbyssaa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/goxskzsfs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gvhkiyurl.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gxaqlyofu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gerpkkjyh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzajmauqg.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gosrieduk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbposyowk.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gzedlgtpp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gpsgfdggq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gaouydupt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gerzyjuwz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gbuohmbnu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/glcqrlorn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gfiinkwfp.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdfwvqmgd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gfmwsxzjd.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/glvcgront.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gbucaonoz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/glafhxvyx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gtozxmzvd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/giyjvhuuy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gbhsinzve.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gkkwtykcp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/glcqzqdbj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gfuzdovmg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/ghipxjhhq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gfkvbjpmo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gswdwrdve.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gltapsgds.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gctivdaix.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gahxokblc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gzvaqcqsv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gtdjmukxp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gcqwsvsko.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gwnembmut.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtrztefaq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gmcdvdaff.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gxnwtvbcp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/givjkrxgn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/ggnfnunsq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/galptgaxe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gbdtzsdbb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gcnctdzlw.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gupfkhbsf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gojxsksby.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glxnvocdv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gemyvrwrj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdqoayoej.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gryjwqjsm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjdsbtdh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggylklabc.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwsbiwdkn.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gzmlitcch.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvbymkots.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gfsvtkhtc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtrfslbev.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpiznlcxy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gsmsxtjyd.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvlurxgrl.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gufskdunj.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxilxxluz.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gegovdgny.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gnvxslijb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gnxfotbww.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gtbfemqds.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/grutzgooi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gegjdnytq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gncmfbinm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gpdbwcbrf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gerziksvs.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gvxxrhynu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gswjfizah.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gjmzjfsis.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/ggrqzlaib.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gipjomxaq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/geodmqgme.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gesgayczq.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gdrrknfqc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gvthuovxg.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/ggvwkuscv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfoewpumg.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/ghnykvwvn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gbwlikomq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gkibpyvev.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gblgqabgz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/ghzirmlqz.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghceisgqz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gjvecyztj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gzealbgup.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfvxrmhdt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghokrjuhf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giuxfwphx.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/goteknbaq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gprgrzgvx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpzkguqvw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gtpoguirn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtnttzwfi.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gqfglsorv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gforvbcyg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gqdjwgpiz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gdxvskwuv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gilpwgdbh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gntvecmiv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gkmdrwdqf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gusskiciz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/glxvddpfl.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gjtsjxcss.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gkzkpygut.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gusqgbubj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gzwoxltqf.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gsaobmsvr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/ggzkmywly.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gfbwpifhf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gtabivuow.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gikckxdni.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvneyphtn.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gbklcqcfu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gevmwfetw.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/guupwzrra.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gbhcqsgar.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gyqpesprp.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/ggnxdsigx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwuavwtpr.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/goynsotoj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gowlklian.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gamhozxhy.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/glrtrvthg.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gsnbytrsp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/glxtoowqo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gsowldpnk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gupdrcgbs.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gjygrcisx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/getrrvczw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gceewczba.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gauxkyscg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gqlqlgegw.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/ggspgyzgz.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gnwxibdao.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gmzpvutpc.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gcnusmhao.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gapwvqdfd.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gvdivtyon.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gqvrqkost.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gxttbkzfu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gjhymaaia.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gltcqmcvb.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gxdtnkrsi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gwzkowgip.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gtzlecrzu.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gogfchgfp.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gwniddfiz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gwbjrjing.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gfilmfrzt.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gdkbyehtn.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/giwodprej.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gsfrajjub.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjiixqsvb.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gwjvtckbf.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/grffugfbh.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gitvjkryz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gyiqrzqlt.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/geneaivns.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gwsoggugr.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gybpcfsss.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gtjvkpcki.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gofdcrbof.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ghaocrjhj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ghqpxhlme.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gtynpovzr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/ggjhktvec.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gfmgberip.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gobdhghtc.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gwylewbwy.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gygmkutpn.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfcklmdrn.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gxyzayewh.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/ghdmisgkq.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gecxgusre.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gvpbkndsk.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gfgjnvrel.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/ghrphmduf.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gvjquntvt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gbuudykqd.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gdxvzqyry.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gatxmaqlx.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gevvqukov.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gwzscdkld.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gcghxudmd.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/glklnvjra.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gmxpupwir.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gjchzgvmx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gwruwihzz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gvmukwgqr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/giiwolybs.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gwcrupopu.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gndhxwfmv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gyqteqwoj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gbuipeylx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfiktfjfb.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gexrhjobo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gfugougmn.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/ghsbftxrw.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/ghhplxgmr.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/grovcwpmr.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gdwaztvoi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/glngeothf.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gsyjcnnep.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gromyuklw.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gkeipeymf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gzapnqlsv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gdrlnxhgq.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gzjhilndx.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/ggdapvwws.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gpevgagbu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gmmrntbjh.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/ghwbrzeqn.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gxzkmawxb.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/ghkxlutqt.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gqjfbiivx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gefhsmorc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gzhulpzww.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gmzhkenvc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gusrwcemw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/glircfizt.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gwqlewchb.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gbxvtrrxw.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gwwnhosut.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gzzyyqucp.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gctuxcabq.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/ghknmlair.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gdxhpwvep.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gjxflumad.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gelzeklqg.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/goptrbwcm.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gavwfrvxp.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gsgxseqnm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gzvtwvhtt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gatebvoqx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gjblautlx.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gychqzbxl.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gbyyyxwna.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gxioccjqk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gvqvolzdp.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/glrlxzvhu.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gjmepjnbf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gikufrsvt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gzaoipagi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gzyztrlwi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gcfsnlutc.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gwxcfwbtm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gfniywmgq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/guzfoivyd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gyznpitdq.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gxgexhowd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/geehajhit.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gautjatyo.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gjiofrczm.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/ghpkmuevw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gnhqrzedg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/ghsbfplwj.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gjgbohlrr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gnqnxwniq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsnfgpdea.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/grwnzadey.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtekirytr.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/guacovztk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/grlbshjbe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxgvilwqc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gybgikrqt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gylgltuhl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gftrcgmtw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/godgduitp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/groszwuvk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gsedqgogw.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gltolithe.sHtML


<!-- 参考信息 -->