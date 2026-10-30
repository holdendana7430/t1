代发 wailian999

Go:   if s == "" {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gruvdstzt.sHtML

Ruby: if s.empty?
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeanfyht.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrhvuhin.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwjiabtq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjtddfks.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/ggspfnwhx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqszqfhh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gullvaebt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gpjdbnbeo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfhwxlbt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfxyzkyk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmvxtwwp.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjysatjah.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gknrftlpn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gxmhacbdy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gatsarjub.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlyserxa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gpjgkswha.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjybytdqw.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gszrvbqbu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjvufvjk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyncacsm.sHtML

F. 文件与目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdidglohw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdujuwcrc.sHtML

[F01] 读取整个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gljvtigsh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fanxiaobao.xyz/Article/details/gvhtagxsz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjdryqqn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkokdmcm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gusvvvxat.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsfooxqu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fanxiaobao.xyz/Article/details/glqczevqr.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdjvvjif.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/grmfnbkwu.sHtML

[F02] 逐行读取文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvwzmejcf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fanxiaobao.xyz/Article/details/gjizyhmef.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvcffzyd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvaxcpjcp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/giakzudkz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapkcpcdi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsadutbbm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjezrmqei.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fanxiaobao.xyz/Article/details/gllqwpaft.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/gnpjmnfbg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gyyveaarz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/glbktbxgu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoertfxz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxhsmjak.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/geqvajfwu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fanxiaobao.xyz/Article/details/gprnizpri.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gfpaybgry.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmxrhhsj.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbunabpax.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjlsphov.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpliimhf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/grebcnlka.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhalrnuj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glielbxvm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gnwuxmrzw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlblqqsp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gtssuqmgu.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gymxslebw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fanxiaobao.xyz/Article/details/gyxkdzrae.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedghpswb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaxxytzq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcfzcqyc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqirjcfox.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/gjxpiibsy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlijmmzw.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdhjqmhk.sHtML

[F06] 删除文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goycajvdh.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gzlbkvzfq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/getamhykd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gjbhsvhco.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjazadrz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpundubq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfultnuca.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbxneirvr.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjblkcnmc.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzbrfsaz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqnjwhbl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjjfwijc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcmalbae.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxjsoraf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjqwgahs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fanxiaobao.xyz/Article/details/gdxswzfog.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fanxiaobao.xyz/Article/details/glmizscpd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvltpyeov.sHtML

[F08] 遍历目录
来源：http://3g.fanxiaobao.xyz/Article/details/gmhapbigz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjutagepd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giyldhyii.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshwobfuk.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gnrffkqls.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/gfkieonbs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gawzawkyh.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gnbtyjitw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdivxwhqi.sHtML

[F09] 获取文件大小
来源：http://3g.fanxiaobao.xyz/Article/details/gxgkaimbd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtklbdfc.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoeaqxgy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyflavmle.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjplefmd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gczanyann.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghadeepqy.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqheaxdl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gplwsvcxv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fanxiaobao.xyz/Article/details/gggtybvvy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwcqwsgj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gprxubfkp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedcoexnt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/getzaehvp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fanxiaobao.xyz/Article/details/germssjbq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrpcsmrf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaovuhvx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gtlsxucyj.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geamyernc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfbzgdaj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/guplfsqgm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gpjzdyfyr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gjjqrftyo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpyfoibd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/gylfrnyid.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gdugvqeah.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqciqufvd.sHtML

[F12] CSV 读写
来源：http://blog.fanxiaobao.xyz/Article/details/gjrbgnlrt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fanxiaobao.xyz/Article/details/gnmbttbsg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fanxiaobao.xyz/Article/details/gmndvmcmq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvfkyipt.sHtML

TS:   // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfdnjgwg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdihxvwxu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fanxiaobao.xyz/Article/details/gljkekidk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqdcmefs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fanxiaobao.xyz/Article/details/gsbgehcpr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaxzdebsa.sHtML

G. 面向对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmcctnwk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guglkcmgl.sHtML

[G01] 定义类
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnrdgwsg.sHtML

Py:   class User: pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbpubpvb.sHtML

PHP:  class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjyfdwxnc.sHtML

JS:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqzyrqcx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fanxiaobao.xyz/Article/details/govogfuzs.sHtML

Java: class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/glrxabphf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghorrvuuz.sHtML

Ruby: class User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkgveeui.sHtML

C#:   class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbtddspal.sHtML

[G02] 构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnerqfflx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fanxiaobao.xyz/Article/details/gtphqnzdd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/geumyzqzc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/guodyvevw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuczjptg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gybweolhi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizlbuwrb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gciztzkmz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpdttxbb.sHtML

[G03] 实例属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbzniwzj.sHtML

Py:   self.name = "x"
来源：http://3g.fanxiaobao.xyz/Article/details/gqfivhqdg.sHtML

PHP:  public string $name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gnnzekqpd.sHtML

JS:   this.name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gxzzirayo.sHtML

TS:   name: string = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgnyjvnb.sHtML

Java: private String name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gddgaauas.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixemycno.sHtML

Ruby: @name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzutefpr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmbmucuv.sHtML

[G04] 定义方法
来源：http://3g.fanxiaobao.xyz/Article/details/gvsnhqifg.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/gxcuwgmas.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuktfmby.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gikugrfrr.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvpxpumlf.sHtML

Java: String greet() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnkbcbxc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fanxiaobao.xyz/Article/details/gzsnuvagi.sHtML

Ruby: def greet; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gryflancz.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gjjijbxla.sHtML

[G05] 继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpoxslfx.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncufyycj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gykzuokad.sHtML

JS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gutxevhkd.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grbjlnvuy.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxyszotw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhdjyeak.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkunkjyzk.sHtML

C#:   class Admin : User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnzkytcbq.sHtML

[G06] 重写方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gakxueuky.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxivyfvsh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsswbbxd.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gokdkhsjg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gldaxmaqo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazguuxzp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fanxiaobao.xyz/Article/details/grrkfipbx.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fanxiaobao.xyz/Article/details/gvxmbsbkw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlwhgiol.sHtML

[G07] 调用父类方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjjrfrvv.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/gezboowpc.sHtML

PHP:  parent::greet();
来源：http://3g.fanxiaobao.xyz/Article/details/giuzhjcia.sHtML

JS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gbjnpypui.sHtML

TS:   super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gurwsotpe.sHtML

Java: super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gixvnbnjm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fanxiaobao.xyz/Article/details/gynljzdgp.sHtML

Ruby: super
来源：http://mobile.fanxiaobao.xyz/Article/details/gloudpilg.sHtML

C#:   base.Greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gnukfbund.sHtML

[G08] 静态方法与属性
来源：http://m.share.fanxiaobao.xyz/Article/details/glojynmtw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrwabomp.sHtML

PHP:  public static function f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/glnkfzgla.sHtML

JS:   static f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjafwhboq.sHtML

TS:   static f(): void {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gsinwxxne.sHtML

Java: static void f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/glymyxrfr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fanxiaobao.xyz/Article/details/gppsprfwi.sHtML

Ruby: def self.f; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gfojyebfx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghelhqvwy.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdbelsjf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fanxiaobao.xyz/Article/details/gesyjlgry.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gopbtyrgs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkywydsa.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmgydivtm.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqdccfhhe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fanxiaobao.xyz/Article/details/gkldhbnfs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fanxiaobao.xyz/Article/details/ghbqcayht.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnbleiuo.sHtML

[G10] 访问控制
来源：http://m.share.fanxiaobao.xyz/Article/details/guxdburhs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzdxhtea.sHtML

PHP:  public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/guxhphqbj.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzhznmbx.sHtML

TS:   public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gppachmqy.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fanxiaobao.xyz/Article/details/gimvbwzss.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fanxiaobao.xyz/Article/details/ghilmkssu.sHtML

Ruby: public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/ghjrtvfmx.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpsahwjo.sHtML

[G11] getter / setter
来源：http://blog.fanxiaobao.xyz/Article/details/gkoecjzcp.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fanxiaobao.xyz/Article/details/glfwinqsv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gykwalkmr.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gclgbpjwm.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gftrabnci.sHtML

Java: public String getName() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnfmnekqt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gccthzcjg.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhjcinuu.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gansdnfla.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkmguqra.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtijlnov.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvcofcqh.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtegofbbl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxliasee.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpghuklgi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gvdqrrnka.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gcylkpprw.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/ghxzmbjqv.sHtML

[G13] 判断对象类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gcucsypgw.sHtML

Py:   isinstance(u, User)
来源：http://wap.fanxiaobao.xyz/Article/details/gejjgqahm.sHtML

PHP:  $u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzzkbomh.sHtML

JS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gdniafpfk.sHtML

TS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgsjsbcq.sHtML

Java: u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtckjgcgp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gejailfng.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fanxiaobao.xyz/Article/details/gkylpigvl.sHtML

C#:   u is User
来源：http://wap.fanxiaobao.xyz/Article/details/gubqvrwva.sHtML

[G14] 数据类 / record
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbjscgsu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdlypkge.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fanxiaobao.xyz/Article/details/gswsjmmyl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwrkdfry.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakcrxmkf.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gunmvqryu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzltprezh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fanxiaobao.xyz/Article/details/gjegndsnq.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fanxiaobao.xyz/Article/details/gmrnhzilb.sHtML

[G15] 枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbeepgwf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gghfmnpbi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gutjotrvx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlxbffrc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnplkbfqy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmculivjx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdygbxjlr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvwujptg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxbhxkpx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztyuevnp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fanxiaobao.xyz/Article/details/gopmkmvza.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdreurzzo.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtttzndl.sHtML

TS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/ggejbpjzl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gibgtfpsh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fanxiaobao.xyz/Article/details/gkfwlukbs.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmxriiew.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaapserp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glcjfecah.sHtML

H. 异常与错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gnheddoai.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqetwlgno.sHtML

[H01] try / catch 基础
来源：http://baike.fanxiaobao.xyz/Article/details/gikpgdlyr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdcbqbzf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fanxiaobao.xyz/Article/details/ghxhmdgwq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqpbyqva.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyqqnzaz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzuddbqiz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gschiovoo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fanxiaobao.xyz/Article/details/gigdtqvcn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwafnfloh.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuqvsjow.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqmrtiiu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gossmzogt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjjryqti.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gququvbta.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwprleipk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grronwltg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyworutr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gcjmfcyfx.sHtML


<!-- 参考信息 -->