代发 wailian999

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gnthlexma.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gbfxcepad.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gfsnekddl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/geyygmgyr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gwggdehbm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gnckfwqxw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gdcycjmqg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gpxhyttfx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gepelzitf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guetpfwph.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gisvnljey.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxrjygcna.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/ggwsnujuw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gjikrnvzl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gyxwltwkr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gkyvtqymt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gjbwieena.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gxjibclfl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gncohkdtj.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkazaqpwp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggabxofkf.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/glexeefwa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gefcxmhmw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gunljtxyp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/glcjetfcx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/geozumget.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gwvgajbcb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gsclbirkf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gztfrmteu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/grcxsjuxf.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gwvdftbpf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gwdxnpjce.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gqcnegmuf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gfvwspoxp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gewtbozsy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gfroxjvkc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gzztfivdw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gsavdfoss.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gqgfhiwws.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gtembijom.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gfdzbaire.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gkwiujsro.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gndfezcyk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gyxnoekqd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gcruurbey.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/ghzythlxk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gymhdgxqg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gcjdgyhad.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/goxcwodca.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gxkzsdsqy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvuapefzs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grvzpcvwz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkhqhvlzf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ghqkdyqfe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gfocviiwr.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkkglqznw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfpnqzfzk.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gadnemqvs.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtudgenbf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ggjaxkgpu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/goufxjevg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggxmamccm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gvxgsglhw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxyalpkoh.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfbrqlmrd.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/ggmezmcdl.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/grtrlkzgy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/ghspylnuq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/glitbzafj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gjybpkbzh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gxegglaho.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gtbkekzjt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gzguxdcwh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/grenvfmfs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gvfqpaxck.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gpwnygiku.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gndcxyrfj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gosnetvpu.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gfoqaonbe.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gwatplomx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gszmluzyw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gtpvnitxx.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gxxrpdhso.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjhkwvefp.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gjnzcvlgr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtlczfmgg.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gezqcfemp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gmeibkdfv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gnszglqai.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gscyfulzl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gjwmpxltx.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnkajxssi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gjsmuqqow.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gathfifdk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gakulkekp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gfecmohmy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gnfnoixgw.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaikzanoo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/ghlqlnyrx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjctovjrq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gopuckahu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpliedajq.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gyvjzbcfq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjmcpubaq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gbsmgwrxo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/glozgbzwg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/glekqmxip.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gvouelekd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gnmmakdbm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxyxdfbhm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gqxmshxvf.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gvdinhgpf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gmtjtbsha.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gtlvpnvec.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gjuzpxtyd.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gsngjsfsw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/geyumchdx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/glppycekw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gmsupkgst.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gdkckcwns.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbfzdpvoj.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gcvhigpsx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwalvvfat.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gekgmxnvw.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gdhunqsvx.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gcpxzchrr.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gsecjykkh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gmpvzttgv.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gncfutkfi.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gyiqsbqij.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gcqspeeif.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gzopbxlld.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gkdfghgst.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gyukusqjy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gpgwgdtwu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gahewvzqu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/grarsljln.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gpavrzvbt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gvktpgyhr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gdljbockn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gbwnubzxd.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gebwfnqky.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gmkucolal.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gcpfhtefk.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/guotwwnjj.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gtjgavlqc.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gmfbrjiel.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gstgdxsgw.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gtxeuotmw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/goljxhbna.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/ghhoiedaj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gbzykmhvo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gvyavtkid.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvclvadra.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gtrilvdqq.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gljmmqjbn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gpuxiftal.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gamdwtbyw.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gnisnzrot.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/guxajmgdc.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gwunregla.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/glbvdtpfr.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gcmmyxtza.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ghovjrxtv.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbfkeypza.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gjmmuleqp.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gquuzlhnj.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/galeqdkoh.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gyswrampo.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gryusfgva.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gyyrsytxs.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/guhhfgikr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfptsjwqe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ghunandsu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gbrnssfdo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/grpnqomsa.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/ggaotiuib.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gzegsffdy.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gadcycgya.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/grmsooqtr.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gbhqhqmfr.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gxyfnfekh.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/godgivqzg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gvsycipas.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gntowelcg.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/glrqwsubz.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gknqyoozk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gsbtygcgl.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gbczgijag.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghbadealy.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gfvgxcjrm.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gmoiccvlr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gyriuadbw.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gvqwcwvix.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gxbuwvndy.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gkhhmayje.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gfxanrgkm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gtpebjitn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gklcggrpe.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gfwoocbtd.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/graswlsdb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gexyyhzvp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gxfqadxvc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghpmledpg.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gmapperzt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gaxgckjce.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gkhjzxpxt.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gqqnvohtf.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gdqxosyof.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gwwpertyu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gtgyevjee.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/goajnqudg.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/ggtkptmqk.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gdsrnsinc.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gijxcqhfk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gibopbqlf.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gpkyflxzn.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gwwiwlflr.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/grnbkjqkv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gnoyeuwya.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gmxltofoa.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gvakykmxz.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/ggyogohhk.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gpeuxmkse.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcisdvub.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/geybeygcj.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gmromoxqo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gkczkisud.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gavcfopcz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gwuusbofv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gjgdfqudv.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gybmkoxko.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gugvfxgyp.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/grpswqsqd.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gkbknbjnu.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gpaxkmdzi.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsecysdlm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gkzkqwftf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gphbhlruo.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gdgtvoymg.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gvizunjqi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gfxlasifj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gxwtwdkxs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gryrtebiw.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gaspgnlky.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/grcuulgus.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/ghoyakhgz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gcpeercxi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/ggfslrygf.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/glmfnyqgi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/glqcnlhfw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gtidypmiu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gutxvdnjp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gqnghslee.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gafqdkotu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/galpjeidn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gaijfuqlc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gjehiloau.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gshnrwcxb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gixgyxydu.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gdbypmnfv.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/goivywoct.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gispfeagm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gfsusonui.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gouzazajg.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gtulsbzbt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gdygemukb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gepbzjicg.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gtvliqtme.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcovrndxg.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gyavhngzu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/ghyloqtnf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/govzxwufg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gjipxfsgc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/glhcvppnh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/ghydbunva.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gaplemrdn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gajinnrmx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gzukbvcpv.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/ggryekarh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gpjnsrrty.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/grrcmlkhs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/griivyvds.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gxquzuski.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmnqsslbr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gbzrhejxw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gyjftadap.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/giidsztbo.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gfjjiaamo.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gfhtuzqga.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gelipzksx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gzfuuamax.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gexrtmprn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gulplmxft.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gataidots.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gpilkhjis.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gfoleeqeo.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gevkklboh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gspdonmei.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/ggzytduxl.sHtML


<!-- 参考信息 -->