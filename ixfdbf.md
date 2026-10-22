代发 wailian999

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mzjjmulf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vvmqwzvb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2fgnjemqq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jfddssbr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dlyjaosl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mlmbznzb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2fesaobto.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pbnexscy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2pemaghez.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ultbgaqx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2egoswowk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wsnuqoxb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wtwswhtb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vkvfxibi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2flfaakjb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lpprqubn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nhtcgudw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2pxocobpz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ykfpjiiu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ohqlggmp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gbietnsw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aynagqxw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2syxglhin.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ycmyhzmy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xzbadiky.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nplplcpl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kpmlrktt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wpgxulzs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nwjulnpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivaphuhc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mssewfan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttprinvg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ucuaxjxl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2uwbedubr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hzpaowhy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ujsubnoq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hcvcmknx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gxnrdghe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vnombmsa.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kuzenjwx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bjrotvtw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzkjerwq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2shvdgkqs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftfowtor.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvkunowd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snmxakdz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wgdpzgda.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ujkdnykz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qbfuodzg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2syulfzqo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2whqmaxvt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wlxhmzhf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uvyhindj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fxbcbgek.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bvsgicwl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2axcggdsa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cvmlqnug.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ejuuqmps.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vtwadhyc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2avjxmxzq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kfyzlaha.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2chzkhwze.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hbwpfzyq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2brwygnop.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lazrjsdw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2thmanxdc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hntwzliu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jwbrrsbi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2lxrvmwlv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qhdulndn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xpdolwzt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxnmelom.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbydwdpk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2raahftyx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2tgjqyryl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uybsjwod.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbyjygpi.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ragixqvu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thtgvqph.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ddihdvwm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qorieuyi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2weyskifk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wininohu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wfcfqqrg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2atecuzjc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ozgqpzda.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2loetafdo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xpcoyhks.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2fbireybh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ubiqukyh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2plmyibsg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2kwvqrctb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ooynnzvx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2nriogcto.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2msyuprvv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mljhyqvo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lgztavsi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbvwaxnn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kgbdxjmu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yhwqvhff.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dyppehpa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mdfgpyco.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rjwnrdsq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fwuogxmn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xpawadfw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2coerhjfr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yqhvkzqh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lkbxxmiq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dphhnzet.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ymfbqbfo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tppckobm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hncolijq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lkpjysae.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2qaqerhub.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ybttrcjb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ijvnoomi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2deayeleq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2muvglkfe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2sgmwujrv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbqwselw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2icuxxpay.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tyvoiqfn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lxktayjo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdvvhcnc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pwnfszha.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aowkvohq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krywexow.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rumildso.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2odqkxexc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksxdwwqx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nfbtwurg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tbqxqlki.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ohqokbaf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rgirnibr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qmrtbazy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2luimutpq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2uqunssnv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2femdwtwm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2scwxtedf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lyvoqosh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oedlpekn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2yrvwrshy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnyabxww.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2iwoilzem.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ddguuhgh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxlltfad.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sjcotaai.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbmigvhl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cygwewji.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2pmmwzavp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dahgdamd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyuzqfbv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qhnmjixg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2kdudvhjj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2kfpipzdw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hcflagxg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kbdxfuax.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tbfeefpl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dmlnnxth.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2tlltxghq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vrucaunp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jbethbpj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xlebqmjc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zjqrmppb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tjtlvokr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2tdhozyyt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qxkdetju.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zlcykivz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lesxqmfu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2rrxqcmdp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lszykobb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2clgoabhd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssdmcblg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zcuoiqwn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajoizvfq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aatfabox.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gopwhhzi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2spszafxu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kaglcibq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xbnsltsu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sibxwxtn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgvrcjeb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejinywwp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gaapfjic.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2btozxtjd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nhjocfog.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jjkzdyeh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zbhyrcmj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2bwjnpbpg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nkaprkpv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pmjizklp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbjkjmte.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgyiwspu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iajxonkz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qaxbmexp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2etklspep.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xuftkmum.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rzssczlv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2vbxtmkfs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2umdipnot.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rtmlkeso.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2juzhnehm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ejzmbixh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fdpipysd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fwndmkuv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dkkrqeub.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2jajsrqvf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2nuzgirhx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2djovovfq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ejlydgei.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqyqkcjc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2olpizhcz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lxtkeugd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wzovkqxc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ehodhqkm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fcwwpfop.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mhyxocqt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylzpqaef.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vebzwdaq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2wloikjqr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2txdkmlqc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2graecduh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2nergcytx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tibaiura.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2yahswcql.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2cwdqsubi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kbjzaqeo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2txywslyw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jndzuhgb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gxicyoda.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2chpjpohj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jbmbqiqb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mqajwdzr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bedwejzq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2krblwigy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qidhgfwz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mfxlutrv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xcvkxmkw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibkuqiio.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yzftiljc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gdtboyws.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsmhrskd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xgtycftw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jvcdrfsd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2esjizkwl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgipjtxh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfhlplbl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fiqiljwj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2apztzwvb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pvudvvrd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dzcjdaax.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dcnosiaa.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vggxjqts.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2icmhutwr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dftjtrim.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2npmwjldb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ndqrazdr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2friuhxcy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2isgizcbb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2fswagfbk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ditzxqdy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tupngkkp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vafhyovy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mbwdgzvh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pxjqdwts.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2usrgnksy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2cktkiceu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hyxrabwc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zopdrugz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xbvaxnls.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rnxfwnec.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzdexckf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2acqdnach.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jgawutyr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xenjxcmt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2unsjnyel.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wnmbezzi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dgyhqghv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dceknewh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2yvegmeut.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2uqcxzbir.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bjmkjkju.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bgdlnynj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2sxwgkogq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qaekzqyy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qqnmprzj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bkdosxae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbisaaqr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ihnztcpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfzvhtyj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2okehjtxl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gthsskth.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkmdybzg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ypcbdttb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2adjbonvk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vlrhbvau.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mjnlkfbn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2rbxikwgw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewjhqcfc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hdosolgm.html


<!-- 参考信息 -->