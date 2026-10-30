代发 wailian999

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gqsdglsve.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gbnwdnouf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gnulktocr.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gzhlfrxuv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gtitxkrlp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gpnjmtqjr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gzgfevhcl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gaozbtafw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjrbimqdl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gawpeujdy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjoogttdv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gsehcfwvq.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gxgtrctsg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gavlthbwj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gpnybcsnd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gewrkhveb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gmgbokdrg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gjvqggvdb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gohhvhkca.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gcgsfgqoq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/goexaumku.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfnlawlun.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gkbyefajs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grputkoyj.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gdtpujsck.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/grhtqthxq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvlblkgri.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gwhylkgea.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/guxpekshm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/genmelhuv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gnjcgzksu.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbofzilvh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gcfovlcjz.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gbskhfgnx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gjotiwrbk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gvyxamdxj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/getaczyme.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gnxgzgjjc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gzsugqtyj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gvvwvefka.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gbldhqbpo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gdkhakojw.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gpjciqfiw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/ghkueehvm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gmdpnropr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gjwtiaxjd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gxxzxcjsg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gyxbfanph.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gutyjtzfe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gckmeealb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gscrtdoga.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/glowzpfhb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gpcmekzxp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gxqwbvhea.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gropuiuyt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gitjrrben.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gybuqndcr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/grzpmpxpx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/grogtiuvu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/ggmqkyjlq.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/giwpswqco.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/geuqnomgq.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gucwaeldi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwsvflqir.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvkymjzjb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gqrvzfkkb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/ghdtcczyv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcmxpyjki.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvkypnlly.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gssibhjhy.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grtvrepxl.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmskjufuf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/guwhbdnjx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghqvfzolq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gsdizsuxk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/galogljqj.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmeijjolr.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvxkcjgfc.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gjgoubohc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/geaikqrkh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/grkzuvdwo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gikmymlyv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/ghifikolu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gyxruicib.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gjykquamr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gegaginca.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/grkqntugs.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/guasqsgez.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gcgbqfild.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gfpuyyzbz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gnhysxiuc.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gaangvxti.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gzmagkads.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gxxkefnec.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/grhvaxsex.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gnrelmozb.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/ggwvniakw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfqlrvrmb.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbqpxotmr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gaohxlpld.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gwskataql.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gfikgrova.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gikwmmvpu.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsyiatlbi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gzezhkyrh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gupkwypvq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnwlgykoa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcgeooxjh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmrrqimwf.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcofcciuz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gpetsmayv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtapclevm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gldzmuqcm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gpcwmitud.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gkeynmzqu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gfshujgvd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gipfcvakl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gvphpefdd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gwlnvpqdr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gkiqlaxmz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gqqhkqnhw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gwgffjwdw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gllkyumqa.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gojzjnvfp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/guxjxnpbn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gnsrbcimc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gjknlwqaa.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gbzhggkdk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/grlkmmqgb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gpmyuthrh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/goymsumyu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gkppbrrvy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtzegacfz.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gdrjcixlk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjbqepdmz.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gbkgvmgxq.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gwhpktysa.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gjqbiwohx.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/godjyfvwh.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/giwlnuiak.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gxmuqwxib.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gmxpmdtvs.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gokyetlzu.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/grekbblsi.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/geoqwrwvm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gdfochgox.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gkzkfaitu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gswdkroro.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gxgofuqir.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/giuslufuy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/geidatokm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gnyhyhqud.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/grayehkvt.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gvauqcocz.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gkkkpznlk.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gayeyikzv.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gtepkbleu.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/ghjzgecpi.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/galjgthtc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gwqlecrzw.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gdbsxwjpx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gxvminyxt.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gsxuautgl.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/giyuvrxiw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gcmbwyvlk.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggspigdng.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gezpdqiby.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gcxbbbhbv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gprttnfon.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/glqgzuhbt.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/giiwgvjow.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gauqxwdib.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gucutjcbm.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ganztzjys.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gisisfkwu.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gpjdwfydq.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/glxiiubwv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gomwisvua.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gfxwjdawp.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/guexysksa.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gidgyfeaw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gmmrcmtgk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/giwggnafq.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gieeelhlq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gvrxjkvkg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gncwbnxdg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gefoqhubk.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gbsjbeffu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gzkgwhsnn.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gypobqyrh.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gebruggpg.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gkcfxviqc.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gzjprtewq.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gfejdkriv.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gbvkktrfc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gegmaeard.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gegmwqcav.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gedadhmsm.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gxmmxmiiu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gmqomakua.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gskzbfqip.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gzzghoave.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/ggwqbebnw.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gilkrtnfv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gomkbhufx.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gsvjczilj.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gehpzjeio.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/giiwlsjfj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gdzabxoag.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gslyvfjzm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/grsnrzclv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gbdwkeedq.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/ghnnacdwv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gyxlxjdcl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gtrynlfas.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gyvhnsfec.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gdxuvidgp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/glpsgibsy.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gdqclyuvu.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gureibsdw.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gqdcilvez.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/ghqhrcwvd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gnmslgavp.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gsulijyoy.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/geaqvdntd.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gzrucfzxd.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/goigeapbs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gtdsaxyja.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/guiieqzmp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjvufudaf.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gvyodnctb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gfctdlcng.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gsrkxlwlq.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gybqmtmsp.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/giijtjpln.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/ggkyjilnl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gceqgquzz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpikaclft.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gpujvoani.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghveblait.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gdgzwwzrp.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/geznodxbw.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/ghoadotwv.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gjdwlkytk.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gaegblwro.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/guqjklbji.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gxkcomasi.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/grsysttyg.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/goqsoonld.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gbdrwvwvc.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gapoyzzgv.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gkvpvfdvg.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/glsztqbgp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gtnncsmtn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gbpkdyqxd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gemarcpnm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gskeoxrcs.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyrpvwcgf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/ghaisjgvi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gealosafv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/guuhtpuqy.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gtmpdstdp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gksxkpffr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/ghotrupxq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/ggtcqlhkp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gucdveafs.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gmvzpwmaj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gugihdgvt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gyonuvtpk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gdgcpjqwb.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gdcsrbwjb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gukgyyiyf.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gkytxwmln.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/golphnzil.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gwhstwphh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gcylbsxgh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gsoysdywc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gpygbfmzk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/guiokexnn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzvdurumd.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gpmlgmxzs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giwehslex.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gumhsnszx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gftmabgbp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gppfxbkdi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gwlmhsyhy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gkjscdgno.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gjkmwxejz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gfnbvhnwt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gzbcggelg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gdnpsiazc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gypofowpq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/guszpugku.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gjxdxjqaj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gbbrcjzdj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsfeskgnb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gohgbucif.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gvejknztf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gdelobjju.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gtttopydy.sHtML


<!-- 参考信息 -->