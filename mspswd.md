代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gnxitoxw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qcrkmijc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qulcvdhh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3psbxmuvt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mzhbnfup.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3svcfgrvu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xveryblk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sinmmmao.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cjdlfafa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipqeectz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vxrwdhrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efcmyoco.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3dkvjqink.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wiyoopvq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dhlbhzok.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wxaefvyj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3woeaasts.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zwefujtw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wojdmidc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atxwgwrk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vvvewoal.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fbquwkeq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3vlnluxcv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dovkmpcp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edjxvfgb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3yvaixyob.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pfzckltz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kwadmfwz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tqgxjkqx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bffpqnjp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3mjrtkpem.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mruvmdst.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wkymoclo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mysoaeer.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3srfsnrdm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aewwbted.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rjpujcpf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yjvaupod.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vrnzsysd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ccrhvkmi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nirvkxuv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3tfxqdqkz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hfvgdapa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oejyqxwx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3qzztxgbj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bbgnhhpb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dnrvuosg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dfvozoep.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fefatxvf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3poxcodit.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gfkkeyht.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umfsksut.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbsajgrk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bwditshf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3shsjduus.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ermiflle.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3albxsdxe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xblyjpfo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wdxnryhk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xngipmrc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrzaeraq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxlrqhhi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uqpfscdo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjrukezt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqyijgyr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uuxsqxzl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3iiquezvh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hwqnwkkw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3cnulnvuy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3edyftahz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3crhsfcgw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yayfnggr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mxhmpwok.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tiviybhy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3edykamwr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3dxbzcxle.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3pltargcw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqgjqwqh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hzimxsdm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fuduqggu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hsbxqvzd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hxfgsxjf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ofuxyxgn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3arixzzir.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3cluauvuj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avwefmcr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yaogpdce.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ivlprmbq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lpqafbwq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3clljjzml.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hmzbwspm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebbpkxjl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ftcgywjz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zgtkfdei.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xihwkywb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qtoqaamt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twdabzuv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ickltezm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3wvtcodqb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zduihqgu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfdbisik.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gcxktqvh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ufmdwfyf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtbzsamz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lxqqamci.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yyoshbzf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztficfqk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pktamhcv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3tjfmquhh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mtvfuwmv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ytxqcdpz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3eixwapin.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3koovmyrq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3fmzjowmz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3djknvlgk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3obigdleo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vduikekh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hpvnkuog.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vhrawewq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ivjkjdpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uoxflsqv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3pbgeftij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgzdbbjv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hmneketx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3vqgrbuni.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3gbhwkmee.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjdknnet.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwxglaia.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxqdwuup.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3kdpxbczf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3utzsqdkh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3liqjdnta.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3geobshae.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3bubuluke.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wdzagkoa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvllukfy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kisdtvmf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zbcvjhop.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3moiketff.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3yapbxujt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfucopik.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3gymxeekp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3yrvtptjd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pymitulk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fdapsjyj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fjbbujfv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jrfnxhgu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gqyvsoxp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sppggzdz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fhqjdecr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3izaxfthc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gbdfrdhh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3givltjxf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltfvwrsg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eoewplfl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtzsytnl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xyhcwout.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3omftwbef.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yecqtbtq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rubymrfy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nvguvvao.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mebikrce.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jzijxgmk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncwyacwd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjeynuvd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3okbblvfe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dpdwsuvt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bvcebmxd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ukbsatgi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3uxmesgjv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrcngfav.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sewxnlza.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bpjfddzf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nalyebyj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mtpulxfn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gzfmilry.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3eisakrsa.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qaeduzjd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3pyweikes.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3famajtbm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lqxxqayt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nhhuicgt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uvdxhixo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vnjeyeoh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3opmztbim.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3yrgcyjmf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qmjculic.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fympnsgd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rwiubgbg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lecsdsav.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3jgimmtfx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3najwbqmx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3njdhhyof.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ppfuqfoe.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3edrxoxhc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3aghxbrla.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mkqvduef.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioxqyoeq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ivpdwjse.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdzbfhnd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qbpompxx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lmoangte.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3iisiaogd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zczequcm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3sgcnwrxm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qbmiwscc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hsyybukq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3uzfxupkq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3efkbwmbd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dhdxioga.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lotbtbhc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aoujphrp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ofywihzn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xksxcedk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lnjczisx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ounzanjf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngsvqmqs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vuubpfvy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnjjfzvj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zmnthyee.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3clhksvch.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kayctmmi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3uaoadsii.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hgvmsuar.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cprlutur.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilwayxwr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lrrruxdd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3spfemfju.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wulxdpnx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nhreckva.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jbwompgp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3snscfjng.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3wbiryavu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vrhcvdfp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ktitlgor.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ebdjgvws.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cmkwkuhi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fxgdelcr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pvnhoxsx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kfyirxgm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fzfxxkyh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3esapbdui.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gpiyyzcb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ujxnymku.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wwdgjlvb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fhkhymwi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cmngutjs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3lhgwjhkv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3swktqosu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dxcqdpup.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dnkexomi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxnfjpyd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3cmttnvph.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vbidelos.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bwmacflr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tnyktotx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vqqjndmp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xspzahgk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3psdpaamt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qzekbctz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3igpfmjhc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nnhifyws.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dvgaquut.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3whmkypas.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3satzegtd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zczvpmvw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3covrlnmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ceaznwsm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ecokdvhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqxujorn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rywqogol.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zzkgvlmy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsisjbig.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcdirzbg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ceqwkkjb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ddosjfqy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ezzrneia.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3leowovmf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qvidktes.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3iupratbn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3mzaoglts.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyfphquu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kckvfhqs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtybtead.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yfzkefxp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3svpjzqyj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3msdttaqq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfzgepkh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yaneoutc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3azkneugc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yabwjdzi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oincydbt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jsoyfups.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qwlpfzqw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fqdkltka.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3lfzxtibk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rllxnpqi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3jvxaxcsh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pqqmyarh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbuasiqf.html


<!-- 参考信息 -->