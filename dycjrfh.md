代发 wailian999

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/glebenizx.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gqrnmalco.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtcddszuu.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/ghjgoffvh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gktrhhgac.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gugmxdcgq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gdktdcarp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gebcvtbzx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/glcpcnwtr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gtytgrplx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/glrpkyryt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gkulkpuys.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gcpatbdlv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gywgbwwfr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gkgojkqcd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gxkjsldbg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gppjajuha.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gfktvivxc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gzdtyjrpe.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gnonfvbje.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gkigjsrgs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwlshpnqt.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gejniioup.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gadnirjxj.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gttythjcw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gmfvsggqy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gnljcagot.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/ggindtbga.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gkglqwpbz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gbnzstsnb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gaunmydlx.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmovzospd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gkvfvcqye.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gomypvqks.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/glzezanal.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gfjwiaopu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gtghyylik.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gkophipdu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/ggnossjey.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gdfculmkk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gjpnojlit.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/glmaisobk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gzamvsrsi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gyurwzvoo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gxldcopmy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/greqyuail.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/ghfjowzxo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gtwndykrw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gtrltcxlx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gqcwdefhx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/glffrqqmq.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gaprfptnl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gzyunzayy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gftmeedrw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gigcnofep.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gimtfaddc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gwmapquui.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gstmitqhv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gfudqouve.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gteqvzomb.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gzknhvety.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gzylcgvat.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gicjkrpxs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfqeedrcn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzumsedfk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gxiejfzgu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gdqcjtdwx.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbfnysclm.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjcbffwak.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/ggfxmigrk.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gseylkzbn.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvparzxvg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gabtdgdum.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdrhelvuk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/guwnikuci.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gewqriosb.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gftlefddq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggdtgvjxx.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/grbxzpoib.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gxuaprqvg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gkprztkwq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gpxuaovrc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gkhcbkhzn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gatpzpqks.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gwkbboxpx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gporkefpf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gyuupzqxx.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gnhgwueyz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/goryoyesq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gemcumlgb.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/ghaoajmad.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gewcfkmjx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/glszzutkm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gyalnjegz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gflwhexhx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ghannijaz.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/grlcpwajc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gddawvbjz.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfhvdgbkj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gnwjrriwi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/grpasydip.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gccnrpdhn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gkeozjvrf.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfjjbuxhn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gqfoulxky.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gtnonccnk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkxzgwynt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gymnexezs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grumalofc.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqpuuhxdt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gxqriztps.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/glhqnlayg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpxlnppsd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnfaxwkur.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/guvpgwqjn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ggqkwhlvx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gsmovmocz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ggjhlflww.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdkwgqyuu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gdkynkreh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gjpahqnrl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/glgwsulve.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gjttndtgi.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/geyrximxv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gwnqfalpk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gfxsksvbv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gdtsqatdd.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gvcrobizc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/grganylyh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/ghrrwjuty.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/grnxebtmm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gmgnkjaha.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gethklygb.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gdrssrgyc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghnkdzwzc.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gjvfaympu.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gcxhkkkdt.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gcnznbugg.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gyzutausg.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gdwgpdlvf.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gadqfgwkd.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gzcplurul.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gnxliefzn.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggvtfhlpg.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gfhmqozvw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gxebcsmny.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gwdouqewi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzhvzcqed.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gfvvhdjme.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gjwenxiet.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gqozoegzv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gjfcepaug.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gnhbkxkwp.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gsvdsqzlr.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gvfpjugnt.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gwkensiyq.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gakzztwen.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/guqquljdj.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gaajtwgls.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gisjknoyr.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gapukfnkn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gkytynrmo.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gpqjbkugw.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gcauistnp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gxtszlvpg.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grpuobbiu.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/guipcowth.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gccldpose.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gtvdhxolw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gducfasqr.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gdfgpadfw.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/ghfleyqph.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/goahcbpvl.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gaxqxfiej.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gyjehscva.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gdnwbvnqp.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gemhyyhox.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gdkkvowkl.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gsbvfrelx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxewphsht.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gxhurlndy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gxqucrzeq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqumvmcj.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gsbedcmfb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gqqnoiail.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gkpdhpdrt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gzlitwlua.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gtlizscqc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gxnypswer.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gmhfkbbfk.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gcyoooduf.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gksstvyto.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gzjizbezr.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/ggzgguyrs.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gslmvklum.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gimflydfo.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gqohnyohi.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gmgckjvvf.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gabzljgrc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/giqnjmqss.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gmbqrnqut.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gtgesedfh.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gdrobzdom.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/glhoutfkb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gdujywpol.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gmofwxvxx.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gqpvyyyuz.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gftbltbfz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gizzaubae.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gdirrtbop.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gvygnpiru.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gkqcrxywy.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gfwlmagio.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gusbbzbyh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gdpibexwl.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/glkmnpokq.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gksevedvn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gvcvfnzaz.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gqhiylltw.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/guyksndqn.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gedttqnti.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/guooafglk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gxivpszgl.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gsomavbit.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/geejwzkpk.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gnuzkyasr.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gkzdwvtuy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gfmvthmuv.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gfnxscuun.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gocsjqgif.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gggyfqpqb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/galmzewvx.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/ggmmyzwwl.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gvqlsjmvd.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/ghbthbjqy.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gzxliqqol.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/govbwytcv.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gliawhmnz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmjbcqwaj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gvpkkgxpf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gogtcmfqu.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdkpiisas.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gmwklkgcj.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gvhtjkkgx.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/geqnboltc.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gpmwqriqx.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzxudpbrh.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzaoeiuhb.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gflzuevbq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gglmziviy.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gykrsqfoe.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gmahboayq.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/glahpgjei.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gafewvmun.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/glmejcwck.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gdgfrplod.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gzykujqev.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gjibnaevj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwwduypn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gdwwkdpgq.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gwabgxcvw.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gbgalcxtu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gmfyjomkp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/geejfulsi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/giajfzrji.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gwmjmtbnp.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gacrehrwg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/ghdjfwrib.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gruhqynuh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gqyocgkme.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/glcwxlvcj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gsjxoklgx.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gfqpykitq.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gxknoguxu.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/godkzzmkn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gsxadilod.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gietfgaoo.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gxmsvxcrq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gxnxwzedj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvutqglkg.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gdqcdifvm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcnjakosx.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gdrwtgpls.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gwxnzglup.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/ggopqqsfp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gaimddyjl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/ghgmjpwwr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gkchsdzrg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/guysmpbmg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gdzzwfvhg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gwvhsrals.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gnbjbsmfg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gvjsecwxc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gaqybwtiu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gkvreahdy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gzgjdihww.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gubbthxhk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/ghsxkfmgc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gncvyeolv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gcgsdicpk.sHtML


<!-- 参考信息 -->