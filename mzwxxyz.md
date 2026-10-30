代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fanxiaobao.xyz/Article/details/gzgphedcg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gqikdxugr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxiboaxp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gztlqhjzp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/geahkafki.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxqvfnxm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcxfdayr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gjeegfqra.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqcrvcwcr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpghvrcwl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswxyhwfm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyacicor.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gxpdjkksv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggibvlmxa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfnmcdfu.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaojtftx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gokujtcjy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkxoapisv.sHtML

F. 文件与目录
来源：http://blog.fanxiaobao.xyz/Article/details/gyfyqszmc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gokoztzro.sHtML

[F01] 读取整个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrodgybb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fanxiaobao.xyz/Article/details/gumlvmufp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdjbmgqp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fanxiaobao.xyz/Article/details/goriwhlrr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygsgotfk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geueyropv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fanxiaobao.xyz/Article/details/gxdlvflqy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwhxhpuo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guirmmogz.sHtML

[F02] 逐行读取文件
来源：http://baike.fanxiaobao.xyz/Article/details/gisjzplve.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fanxiaobao.xyz/Article/details/gztrkthba.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdnxmjkr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvdffbwu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjwyetide.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gledynqxj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gabcoygpv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrokguzm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqalplrp.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnkfhhpg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fanxiaobao.xyz/Article/details/guueqjqnz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/glnmjyldu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gibqlyjqj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gekacwblv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gpozjozlr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fanxiaobao.xyz/Article/details/goxpsbpyr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gldtrgxxr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gshnyfvpi.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhkyfopm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gishihhoi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fanxiaobao.xyz/Article/details/gvtuznksr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gsvjrzhhi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gncokvcgf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/gppgtcbpw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvltrbns.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpjkgmgk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gosgskiht.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gvxmkwyqr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyluotuje.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmajmohxy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gptjcbqch.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/geffohrlw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gautmjosw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlxhhqnu.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfeyopoo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpxakgfy.sHtML

[F06] 删除文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvdoimtav.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvuoaucn.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpiodshj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/goynisezt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gmjksildb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gzamehutc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxszkbfk.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gjnpfllhq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkdclcwr.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/gchbdzvnl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/guwfksfxt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/guqtwphqd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gochmrpdt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwcemoqb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gckntdkis.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqjlumwn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fanxiaobao.xyz/Article/details/gynlmltdx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzcpfpqa.sHtML

[F08] 遍历目录
来源：http://blog.fanxiaobao.xyz/Article/details/gjlhoufmi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fanxiaobao.xyz/Article/details/gkxvkvzgl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmjayhdn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyslxxrs.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gepllgwad.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvehpiitj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevtphieb.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvjmjotb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/ggckayoke.sHtML

[F09] 获取文件大小
来源：http://read.share.fanxiaobao.xyz/Article/details/gutlamayi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxpmhnec.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gbihyqbbl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/garccjpjc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/ghprurazx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbboivwgj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjamnknhw.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gttjofkcr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gctpuhups.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcgvoltl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlchxpki.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrdmqhmo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gszvprsry.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhccldoa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fanxiaobao.xyz/Article/details/goweojlrr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmwlwmym.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjdprvpe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyfgulmr.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgnvdejp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvcebvfo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gzchgpjle.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gikjmmnqe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomeuhead.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gsreprpkp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fanxiaobao.xyz/Article/details/gmihkxhwz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gvulplrui.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fanxiaobao.xyz/Article/details/grssbaein.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/gjmkpuzze.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fanxiaobao.xyz/Article/details/gdqtmtcxv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjzabswc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fanxiaobao.xyz/Article/details/golkuqxvy.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gfgwltkht.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fanxiaobao.xyz/Article/details/ghwfqefea.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fanxiaobao.xyz/Article/details/gydzlziod.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fanxiaobao.xyz/Article/details/gbuufohab.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fanxiaobao.xyz/Article/details/gysokkyyw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcorkeovo.sHtML

G. 面向对象
来源：http://baike.fanxiaobao.xyz/Article/details/ghjdhuufm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gttrlpggg.sHtML

[G01] 定义类
来源：http://wap.fanxiaobao.xyz/Article/details/gifwposuj.sHtML

Py:   class User: pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzdayiny.sHtML

PHP:  class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvrtjyozy.sHtML

JS:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpkosayw.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gupgoszby.sHtML

Java: class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gourczacd.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxtjyqwm.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gomxsidzu.sHtML

C#:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/goebpxucw.sHtML

[G02] 构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmqlprxaa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfxwgyck.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gdowcvvsi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gommkjiyu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusrrwuzn.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gscqoumho.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gefrwsbtq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkalntzxf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gunwbalew.sHtML

[G03] 实例属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkhjknte.sHtML

Py:   self.name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gnathpuyy.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gekvehlls.sHtML

JS:   this.name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcjqthib.sHtML

TS:   name: string = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gguilmrrc.sHtML

Java: private String name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giprlktmo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqwcmpnr.sHtML

Ruby: @name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gjafmngum.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzklaiyr.sHtML

[G04] 定义方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjdydtdo.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fanxiaobao.xyz/Article/details/gdfuwlmgh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzcssmbzv.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfuwqpqr.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gumxlscdh.sHtML

Java: String greet() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjfvphwa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwrgdxdl.sHtML

Ruby: def greet; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gwxzxfmbt.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgtasiph.sHtML

[G05] 继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gffpmnbjd.sHtML

Py:   class Admin(User): pass
来源：http://baike.fanxiaobao.xyz/Article/details/glxgfcqsx.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmsogskbf.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgbdehdk.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyuwvwro.sHtML

Java: class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghqfprqrf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fanxiaobao.xyz/Article/details/gnxadbjuv.sHtML

Ruby: class Admin < User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gzmlslqmu.sHtML

C#:   class Admin : User {}
来源：http://wap.fanxiaobao.xyz/Article/details/guanqpyrf.sHtML

[G06] 重写方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmliygux.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fanxiaobao.xyz/Article/details/gypkprehh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpzfyvzld.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpysxswup.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/guyewykrw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxgqxeuy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fanxiaobao.xyz/Article/details/giptnnhqe.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fanxiaobao.xyz/Article/details/gzcknehhj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fanxiaobao.xyz/Article/details/gbpadqpsf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geybcopyk.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkttmnzw.sHtML

PHP:  parent::greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gdcwiynuc.sHtML

JS:   super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gmnzbcuqr.sHtML

TS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxaqsvns.sHtML

Java: super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmfipyyu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveqmznvu.sHtML

Ruby: super
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdxuwtot.sHtML

C#:   base.Greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkysplybb.sHtML

[G08] 静态方法与属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gntqliqci.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fanxiaobao.xyz/Article/details/gqublbppb.sHtML

PHP:  public static function f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkemxsijj.sHtML

JS:   static f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gwzfvrifx.sHtML

TS:   static f(): void {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfjtyjxj.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gutuhsodl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwwmhxly.sHtML

Ruby: def self.f; end
来源：http://3g.fanxiaobao.xyz/Article/details/gqrbolimr.sHtML

C#:   public static void F() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgtldcik.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpkyoxeh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwgmjztf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxmyooooy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprlexxcw.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggnbkzsot.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gdsvblcnb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznditaxg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlsazbtp.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/guvacgmay.sHtML

[G10] 访问控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/glumeibds.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fanxiaobao.xyz/Article/details/gocluhtil.sHtML

PHP:  public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcyfwlqa.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcrgyugg.sHtML

TS:   public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpqusljp.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fanxiaobao.xyz/Article/details/gbqwmecpi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fanxiaobao.xyz/Article/details/gphvmrtic.sHtML

Ruby: public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gbibadlly.sHtML

C#:   public / protected / private / internal
来源：http://blog.fanxiaobao.xyz/Article/details/gjrqbzgym.sHtML

[G11] getter / setter
来源：http://wap.fanxiaobao.xyz/Article/details/grztublwz.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fanxiaobao.xyz/Article/details/gwhingwkd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/galxzzujg.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geptxhsbz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gegdlgvaq.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcllahin.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfidrjiz.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fanxiaobao.xyz/Article/details/gaabjlhgg.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfmyukefz.sHtML

[G12] 对象转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gyjnoqyjc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtyhrwqh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxavhjsfs.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzgvzsuh.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtgnwgim.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/glqmubbpn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gserfuyrp.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/govfipelx.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvyqfaxg.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmftqvqro.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gadacktjl.sHtML

PHP:  $u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gjfbquoem.sHtML

JS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gmpyzzaul.sHtML

TS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gicrkaran.sHtML

Java: u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gobpemwpx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoowhawu.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fanxiaobao.xyz/Article/details/gwmpftndn.sHtML

C#:   u is User
来源：http://3g.fanxiaobao.xyz/Article/details/gcqyonhxz.sHtML

[G14] 数据类 / record
来源：http://wap.fanxiaobao.xyz/Article/details/gjwpusuzr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzxbdufw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvuysylp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fanxiaobao.xyz/Article/details/gfwqoyffg.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxifsfdzc.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhfrlvpv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzltdefz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fanxiaobao.xyz/Article/details/gufstwcjv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawouxlrh.sHtML

[G15] 枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgsryqtl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnpbujov.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxllbvui.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fanxiaobao.xyz/Article/details/gxigacapw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkitbejuw.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fanxiaobao.xyz/Article/details/gtustjips.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/gwuickwlh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fanxiaobao.xyz/Article/details/gstzneudq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmshmihbn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfbfdbin.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnquibes.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fanxiaobao.xyz/Article/details/gpxfygluz.sHtML

JS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gawgvdmlq.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiauhjld.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fanxiaobao.xyz/Article/details/gcpsqszfl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdizetef.sHtML

Ruby: obj.instance_variables
来源：http://blog.fanxiaobao.xyz/Article/details/ggvcnhizw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqefraxt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzlzltvk.sHtML

H. 异常与错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/guhhrzqle.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gardfxuem.sHtML

[H01] try / catch 基础
来源：http://read.share.fanxiaobao.xyz/Article/details/giefebqba.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fanxiaobao.xyz/Article/details/gnleonnts.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnahcdwq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpropevsu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmiuxlphc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpbayepsv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxkkjtrf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fanxiaobao.xyz/Article/details/giftdmjik.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdldckzdh.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fanxiaobao.xyz/Article/details/gqnlysbwc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fanxiaobao.xyz/Article/details/gedentfga.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsxgxbqr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmrjfjarf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzhwyamwg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwpufuny.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fanxiaobao.xyz/Article/details/gpljrdmet.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqgdaoxh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/guzfopwrn.sHtML

[H03] 主动抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gmugildva.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzrdxtmb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsnkbxnl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaaqdrhq.sHtML


<!-- 参考信息 -->