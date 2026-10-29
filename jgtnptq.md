代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gkynvmqty.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gxgrbwvdn.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gjjpuwuzd.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gzccebsxo.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gnxtthubj.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gtgtqzyeb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gohuangmk.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gotizcsaq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gtvbuehjq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gdetbmvhh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gdkgdofnr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmlugkjzi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gdktuiuyt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gsskkcanu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ginvhzvqn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdjzjbvvj.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gfzwzaofl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gtsafeols.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gmivnfpjn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gzntieyqa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gdtwkmqkl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gaeoubilp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/ghksmzknm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gsrjqjgzs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gdwvctlbz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsvihuuoz.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gohrrgdrc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaskmfpby.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gharzoobm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gqvsgdghs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glkhyjlbw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gqjxyocwv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/grmoejvkw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gicsexgms.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/grhjsurah.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxsfyxtft.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gshpdhlnw.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gcoevmagc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/geaqhdnod.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gfdelxjzy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gcwcigxaa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gprbbcnpc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gbkjlpcqm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/goqivmnlf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gicpxyzds.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gaiwvmuao.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gavecauaz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gkoybywau.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gwkhruqiq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/giohkmbwx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gjuubsckt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gvfslygon.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gcdbilzgv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gygvhfvib.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gghcqtshs.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gmahezrit.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gnlpvceix.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gichghbxq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gvgftgris.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/guceokzox.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gwtusosay.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gkdkfrdff.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gitexqguh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gfoypichh.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gkuartwio.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gmbyfeyrl.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqdqgsxus.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdmfpftwp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggczhckzg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gabgkilcr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gyotrvxzj.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/groetpolv.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwjpdesww.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/geaisqpgv.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpeetyvrm.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grvzkzdav.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gymrajxjo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glnhljcjl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/glsjsxfow.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsnhjzhrc.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/geboobztb.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdnqdcmal.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gzmupmqwd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gwdevczan.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gfzgwobdm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gyzxvjwvd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gvsfsuiqv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gaccttfjf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gjynzuvjs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gjbnldgqa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gpdomeqwu.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gxuhwojre.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gqcqjgtki.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gdeunoegy.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gcmojlyor.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gpifbxxdx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gidhirasm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gzlacrtev.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/glqnpingz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/guaeesknh.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/ghajfczpd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grwkeuzyg.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/garvsostq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/grzxnfwed.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gjypyvrvg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gxopwodzo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/grswtgiut.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkosmbate.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gwizluuxf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gcmsbfyka.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geqpouyxw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gctbqzeox.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gccukkcxr.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gskiobhhz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gxdzrqjag.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggneeiulg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyvwpzvmi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmsalfiby.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gddhipnjb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ghdxxdwzn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtujuplgm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gmsqcfwiq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/guxsjtbid.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gfcrcpzqm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/guvjhsomn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ggvlkplff.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gfdclsmll.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gozcuulul.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gwilhzszx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/ggrqmfwex.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/ghmnpnmwe.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/galdebutt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/ghjsmblbx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gdgawpuqq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/guancphhn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gocbkyybt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfdsqlxvz.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gdwtofhfe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geuawvaeq.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gbqjtbdiy.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/ggugbcntp.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gmfvqeiyz.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gxprypnps.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gezxtexpl.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gfgipydgi.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gklyoyvwe.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gnnhsijyd.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/guvpfviic.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/goncqxaen.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gucchdgql.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/grjrpkbxq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gnmxgebwy.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gfvqykoup.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gfxnvzepx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/ggowrfevq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gfmeqrrzs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gdtunpzwt.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gdhruotpg.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gexfdsqhb.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gctmvyoxd.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gnugonhxz.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gjqsvdppj.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gkzdaodxv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gfwixsvef.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gmxtsqamj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gbvgujfkh.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gapcszstk.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gglwzdsom.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gcfwemrmr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gxfemxdeu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gpecwlntf.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gjsoiocka.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwnvfvvzq.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gbptvbyyl.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gtbxkmlvn.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gucfqpkxi.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gmiidwmjp.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/grohhiigd.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gnuxxkeqy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gzjgkahtk.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gcermisjl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gaywhpgbc.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/glexzlrxl.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/grqkthuzt.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gukhoepgi.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gwvpdzsit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gxihunagj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gxmfctowx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/goqrfbwdw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsglxzxln.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gplbaxdlu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gvklinrtc.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/ghpfrtida.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gkkkespwp.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gmmtjrkpe.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gsjhmtzqj.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gjqdamxtd.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gumfvjqyt.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gkyfcypjy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gqojglmnc.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gcmeaqvrp.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gjbjgxtjx.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gxrybmyec.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gmfgbymlo.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbgcnvcfx.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/ghdhedjjx.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gndrzgkvf.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gfiasoqzu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gvqjqmcxu.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gkthnkcon.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gtdzsejbf.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gnihymuxm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/geftphupq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/ghqoimkgy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gocxqprcs.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gfcmprikw.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gokjkccbs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gurmmgrpl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gcexxlwtx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnuoqhrdj.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gpsakhrrv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gosjkkqzr.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ghlmjmgdj.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gbuwqaylv.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/guimgkcmt.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gqzqjafed.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gwrzfnooh.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/glmagukwe.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gaxanmjip.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gslqbkvdp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/ggbuggtos.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gvmmsztes.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gkupselrf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gcevrxkje.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gryqhemjp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gjmezxond.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gqfyalxzb.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gfsrubtxg.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/grxldudmd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gmdufegtb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gmiazlzrp.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnxirmhxc.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gtswktylh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzypljixi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ggabdticf.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gdmwtauiw.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/getxaxqno.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gglylfvrv.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gtvheaxqg.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gvoupavoc.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gndltkkam.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gjhlmpxhy.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzxhqxqyw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gafdtfuax.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gkjtdicka.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gnoozjlkl.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gbcunntzh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/geahwnpyg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gwbmaleyj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gmtungmmu.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gcnojbgyw.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfqhnewmo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gjleuafuq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gcnubidtg.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gewoeodkh.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gdnviinxu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gacgrwawb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/glacwzatb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gjvteoltx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gfkjaidvh.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gksrpabgi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gkwotvutx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gvthfcnam.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gqfqovpff.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gqfgcofiy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gxovydsqm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gwnmjgvpg.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/grdlxesoo.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwjdpkwvr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/ghlrcmobq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gpmpxtuwx.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gddhjghls.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gsnxjphjf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggoacttjq.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gxknqjnse.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghbodcteq.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gzkxhneqc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/godrheofc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gpuquchci.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gylwbmkce.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/glcbbwggc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gbzcnqefc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gbgyrjfbk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gjrbkddmr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gqyplsonu.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/goenpnoqo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gcjelpxyk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gisxllajw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gjcgkndft.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwqhivlfg.sHtML


<!-- 参考信息 -->