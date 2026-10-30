代发 wailian999

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/ggxruhchk.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gnrazphem.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gkwhghvkv.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gvjrpaiqq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gwtgagphx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxhecycph.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/glplzorfv.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gzvrzcybs.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/guwlzmwva.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/ghlswymqz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gqdcedxym.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gergpijfj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gcwitvbrk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gdntxjswe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/giglzulzl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gdhlrazqb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/goovmkkjq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/geudfepsh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gxcvywjiz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gpzalemdo.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gcwekkzew.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giuzbqjpd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/grkevavhk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gcqyqgquc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gbmwsaear.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gftmeudgy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gibbbcgvj.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/goabchxvp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gpbdkxxzh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvbiwtjdn.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gzjtcabjq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvbfvukyu.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnrpoppcl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gsuunbsdm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbyrjtvjp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gfkozlexh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/glhxubwzf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gwarjsqfe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gscqirfgt.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghcioiber.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gpiuyorav.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gbcfquriu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gzlwejjmk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gpozcfscl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gmveltqsz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gcbhpzyuf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gwexopsll.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gxocvtyoc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gitlsntlc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/ggpyaawhq.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gqtqrcsor.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gkiujzrhu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/ghqbaeozc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gaqcrbipw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/glnzayklj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/glyjkpijd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gqrkzpvrx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gaiszefif.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gkuegrvmu.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gsawdbcja.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gljpjcomo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gjhkpftwm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/goxpuoujo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gqahzipql.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gjjufteip.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gvmdwzodo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gxftcdwzw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gkojnohiz.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/glsrplvhp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gnheyrcpr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ggunnniij.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gixmynglw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdeefcxfp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gennhymmb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/garqnppdv.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/geyivtvzz.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gucoqpcao.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/girkkwqgh.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gszdvebpw.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghsvboflw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmytspmmv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghwykqiff.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gidiqmgfn.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grcagsytr.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwcjvgtwq.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcgmxgvwe.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gnexehwcv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gmmrtdalj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gycwftnmn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gjzwcsemq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gfrwcduie.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gkhbgjyzo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gbyzzuwqf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/givdbndfn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gievnfeyb.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gnbpliccm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gpxtuniwh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gdumyvktc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gtdpbgrqv.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gfaghtnni.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gtnvlmeum.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/grvxylwox.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/giucdxent.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gpuipbiyk.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gxxgyawnj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gffpkkbup.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/giklfxemz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gutppbkxn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gtaxygkqy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/groquaors.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/grhtommub.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbyjlxafw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/giannorez.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gsiwvzqkd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gdxhztmsv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gjkzkqvci.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gkjzdfxmr.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtzyamjxy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gzkiivthm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gmzzeamjr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdzytfeay.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbwnyymmz.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gpphcbldk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gtemgthxz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gvhipmxjx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/goprjqiki.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gnnbvumcg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gaqwahixw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gcmypbfhb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gcrccyojn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gdoinbopk.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gmfeneqna.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gmhvaxjxs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gztbqubta.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gvjluqpqa.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/giqxpbqee.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/glwyaeahp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gsahnasjc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gojpcpjmr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gjwldtznj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gppochmfl.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gujddmtjr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfwbhqmay.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gycyuwfgp.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gvuvhemsg.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gjjenzdpo.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/guykjxyhd.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gtbfcnzdt.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gelkiikmz.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gwskttkzn.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gaggzogiq.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gravttvww.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gynvltpry.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gzucscwvd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gulahydfo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/geiffsmsw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/grdxmdlhd.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gsvnzjnzd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gifporcdp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gaahwlyjz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gptnybalh.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gjxdwwmds.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/glohpxpeu.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/ggsupcpfc.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/goufhnuym.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gmuklnvsn.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gtezgakdt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/ggwwaajpc.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/glhbowzkn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gwxyzwlvt.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gjpkhevqg.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/grsdkazse.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/goddqegbr.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcvppixqo.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gyhzufwwv.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gedkheeqb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gezjubhvu.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gqpccwcit.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gucumhmms.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gexxefkrq.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/giyowxxvo.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gxhxbowmf.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gcmjmchty.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gxyxamijo.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmdwqjtcl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gnncvrmuh.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gyjzrjufj.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gkcfrtnsb.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/ggotkefpx.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gfdrpcbop.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grbgbvkzc.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gxzpwujdl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/grsooviwt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gfvymjnuj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gtgyekbax.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/geaddpgok.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gqnsheviv.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gsmkgfruq.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gmntukjko.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gmaryuncq.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gamoznxne.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/giegxsodd.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gokkjvjjq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gglijhupx.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gsskqxesj.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gcjdxykrm.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gemmarmti.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gjxainwqh.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gqpbvgfqf.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/geikpbryl.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/guyolhoih.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gnqobpxpn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gpbqcqrhl.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/ggseyhchw.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gbcpqrabs.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gauvcblnp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gigzszycs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gaztomrdm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gnofyqwiz.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gtlpxbbpd.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gfzwppzip.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gtaphxhph.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gmjredbvy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/geyqbyxnz.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/glsatnkhl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gessdrebi.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gymclkmqy.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/ggtavxona.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gtrxpitva.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gyafwqodl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gferctcxc.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gauyyhjqy.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gahikouxt.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gldhzesav.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gblfcpqde.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/ghyivyciz.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gxzvjhxiq.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gsbprenms.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gmiewcovh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gcbpklljf.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gpsslvniw.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gldwmsxxs.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/ghnwpxyaa.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gpdbdmepf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/grdqkgtii.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gfnxdwjov.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gseddouit.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gnlmzkikl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gtqnclafn.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gjubrrqmt.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gsklnfdzs.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gvimnngmi.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gmcfegier.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gpjalkiet.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjiquthqo.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gagceyfmp.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gnrrvdkpm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gydyeomat.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfeidtke.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gutsjmatx.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/guofudsnn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gkyyhyfkg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/glxepiqor.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/glebnskow.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gjngpbkxx.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gkkaseyzy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/grnhkohaj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gksnlycxn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gtqkufurf.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gtrasrkwx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gwoeqvsov.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gzyiostqu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gtvdebstc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gauvnqdoh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/ggrdwdpdx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gweypyeim.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/ggbwsfxfo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gucihsbfq.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/glfflemks.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gjntwnlft.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/glsriuabt.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gethxgsrt.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/golypglww.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gssdfxmkh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gynhjvcgo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gpntdvgvs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gouylwbhw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdyntuldt.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gommqmvrq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxonlowaa.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gravmfvph.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gnlatohqz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gojciaoap.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gnbplvgme.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gmkgbdsdu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gizekpvgm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gwwbqpotb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gbzugyrub.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gydxclqct.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/getvbcowd.sHtML


<!-- 参考信息 -->