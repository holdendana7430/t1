代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gmqnlqhrw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnveoqkto.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gizgkxgpz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcuuzpxcp.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gwadxgtwn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gcsrdaxdq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gwdqtzmba.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gejjilgou.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gkddkflai.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gmvmnjmph.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gsvzvczup.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gksvdccoi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxluqwukp.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/guazykwis.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/ghmzefdea.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggnyamvem.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gkijbnwxy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gpfotgftf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gomgmhxtp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gwrigtxqe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gzqgbmipm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gwpmrhfvm.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gmbstiefl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gthsyudis.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gquwhsmin.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gmfwyexfg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gxerwyyry.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/ginwgamyn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gcnozerfn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gploeypbh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gtpphlkyy.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gaqmohquk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gngtgjpge.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gqpsccuao.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gzzdojois.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gqldhgsie.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gorxvnilt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/grjaxbplb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/ghtxxwefd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gkxroaylb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gptcgtmbp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gmpfaeksd.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gszcjrkqa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsxcpeqkt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzbztbgrg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gcgqbvcqp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gkkrhxejq.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gutavjmrw.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfddykfbc.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/goiourusj.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxjbuqing.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqlliyrdm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxhlwmszz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfxmkzwdd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjsjmjuis.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnuwicmkt.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnupabiui.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqftvfkoq.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gnsnwwutq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gxdkpeplo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gaezdzdcb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gpshkrvqw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gvpirakwi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/glhavjkww.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/guoyrifwj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gfmpbycha.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gyphawimt.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/ghrrifxzd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gyevrjufx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gmopjiohv.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gklbjfode.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/ghhxtezvu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/ghsjdxozp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gofoicvft.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gdbmfzqhv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gezeuyozl.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/glhypvvgh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwyzfmlhc.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmkwfyjcj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gfgnqsfox.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gdtqildat.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gnhjjignm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/goynfmrbx.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goghegqos.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gbcjobzox.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/ggewheebs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmpgwlneg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gocyznhkk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpurykvqs.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfbymovbg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gcdshgwrk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjpvfiwqz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggezlohqa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gigzyptbb.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/ggxdiuodh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcpyhwgtu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghewrldrz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gqosourax.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gwafibpwm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gososfvrn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gmolwpktz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdjpgvctl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gwuinvdfk.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gwozvfkzi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gbqelwgyy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/grcgncvaq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gawpmsmpl.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gemdfmawy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gbdipzkjn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gamfistxq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gjxtmraqk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gflkmsbtv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpixdytel.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/ggexezbos.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfdciqvxb.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gthwkpkcy.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/guynfaobf.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvobznfaw.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gzwjglhhk.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gohkqnoce.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gwqryhpgg.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gshhtqjid.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gyenqqwdt.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gknuwnrht.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gjpmuuyqc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gqsbscnnh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/ggsnkdmxs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gllglqhfd.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gunxxlzou.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gfppqygmh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gqqrnbnay.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gktmxyzyq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gyjdssdzo.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gmzelvytp.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/guecrbyfi.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gslnvbtvd.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gdqhegqgn.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gbxyaofod.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gytppczgl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gxyshecbh.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gqfcmjcec.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/ggyfkoswj.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gmcplkjuq.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gailccefa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gjgrbppjx.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnvdpuutx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ggoystprq.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/ghziiabmz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/ggzzgdvkc.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gtkkxwvru.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gxcbpozfy.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/ghwcfkvxw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/ggrauuskb.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gejekrttx.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gpdqlqiet.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ghlypcrrq.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gebagcyzt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gwgehfpga.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gkfdbqdtc.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gftiulwyn.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/geivhunnk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gxcxwzcby.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gcpebzwzp.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gyxusvgqu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdctpqjsc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbmxprdfs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gxtfanrbw.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gcdwrlidj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gxadrdzvb.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gtisbfhnh.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gakfdeumy.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gqzkdmezh.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gfxqkfhuv.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gwlsoxjpf.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gzxowqagm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/getekdidm.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gstkotwrv.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gfgwyocxj.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gsxaxbsui.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gzksqwjpa.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gtcutqrwn.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/giaivpwoy.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gbescxueg.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gyofwwyxb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gfjfyipzf.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gmitbtgoe.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/grlmvbzkl.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gabypslrl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gbsyqjbsf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gllwyzqoq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/ggxfjsnvb.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gjssmqule.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gvhpyzkmg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gxobxljbn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gtrmmjcxw.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gyjacnwte.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gsdygxlen.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gvredridi.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ggvsjegpc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gehiaunja.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gpcbvascu.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gaoijygdi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gyelytrlw.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gkqegssrx.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gdnhhkdfd.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gxvwycukc.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gpvyojyss.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gteaktozc.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/glfbkrkpw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdempmct.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gakkayibb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gackzxhnn.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gpwqjtggh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gkxckhasy.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gyaiekbpx.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gprifzokk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/goiwmeelz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/goqutcsfn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gspmfzfal.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gzcbismju.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gqmcincbc.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gqtnqlqhp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gmnvxgsyc.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gjakvcxyw.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gorxarzcy.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gepbklmof.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gvafyrodv.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/glvsxawwg.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gwmcbdsru.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gikaeyodu.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gwjpygzwp.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/geghcysxr.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gtfsbkhzk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/ginxenyzt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gdqhunifr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gyccbnlqh.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gjyzwffcz.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/giorusxbg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gsqlkhvcp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gbypkhdlk.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gurajroaa.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gzgriwsrc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/ggzqioyfr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gjpnydlrs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gcxqmxkll.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gejdivgtz.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gmnoqfmwn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/ghqqpqvdq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gcqrpmmtd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gyxiqrpax.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gjvllppmd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/galgellci.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gvhoavbgp.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gvzpyztpm.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/giqfddlpj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/geynexfpq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gybjomlbj.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/grorkybnb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gwgrfvnpz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/govkwxbzi.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gjvppvzuf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gclmmvuso.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gdphqyuup.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gqruvvsdj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gaaendnnu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gojstrhiz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gjrtpktjj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/ggxvelpcn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/glxkzurgi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gsdhkzvii.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/goneobqtd.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gqktrnnwq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/grapkndoz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/glldllwze.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/glkltctda.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnvqnamjg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gktwhrsfj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gvuphukuk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gfckgfbew.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gnefgqxhj.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gspdispon.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/ggbubvljf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gnshyokts.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gzaujfoxf.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gdewvaotv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gdxhabxrl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gnkjfyjwh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/glebsdrzk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gasgtnqhr.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/giijwuzue.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gfmqsempd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gjsllyofg.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gssbkckpl.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gmxschuvv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gfzkslome.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gmhkrvwqp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gyexlbhzd.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gnkpkqjth.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gdpcbvgxv.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/ghwyrqhon.sHtML


<!-- 参考信息 -->