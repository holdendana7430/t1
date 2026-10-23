代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3syuynjyt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uturwgln.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xpsisyon.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wnodmync.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vpokimgh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3uyurxora.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3szvykykf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3nadmgtam.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ffyxndjo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfewoofu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ceqfvlgu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ozmckazy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3dkdxgowr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3winmbbgp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqofabvm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dufgycid.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lxpodbrk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mpvwoupj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jqglyejt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dhqgalep.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oteglton.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qaryqdzv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3serjcacs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gcnssvon.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fjujydez.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zgzpzvqi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tsfxbjtd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3abbaocbf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3moiqmgau.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pnueswws.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rtprzuta.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rjnzpmsw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mnxkkgiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijrzfily.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gumbugeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohjtsngt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ifyptehk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ncvtnfoh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xxibzjen.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nhuvbvkj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rnkuxzzo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3acwxmvyz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3drldawhl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ymbzxbst.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uybjxygg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3tuppqeoj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ojjwcobl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjhspinn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ongagleb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mdeuhqdm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fkclhbba.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3tbqwvyur.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qgagsvgw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hnbptrmv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wjdfvkxv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wftnyewf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ngfkvxon.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3alrfslxu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3czxqvprl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xzwimpmu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3lnlbgxxe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cmpeqxxs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3itqsyhew.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qrvevyvr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ilnwyldb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3yajgbmzo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uwtygrbt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kikzztve.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3yifiandy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nwkaihkv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vfohupkv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ygpubzqo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vpbnyijl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3deujsysq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jtivsmpa.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ezjlmdyz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulfrdhbg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zyzblrnm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nzwzekyn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iitqawnn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bejbyjqo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3trhfkmja.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wsvpljxt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3abbirmtl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sylyqebc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nkkdvgcc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3epatziqr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mknqpzdd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrlxkgih.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eqcreblm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xnmbpefk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rgrxldsl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tvatqlsf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mrnssweo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bzhknpka.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zqagmmfc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zmuobnzz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fwpleqth.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cevuqckk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3stiaiurg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xfxjqgrj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3mmnjenuq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3psgezack.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yfkmpjni.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3axnpoaim.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3kzisecnd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3rpbtjhvz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qyybrion.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dubddbak.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvpyjcme.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bfpwskrp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kcnxonjc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qyzugbvs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3emjnnhbv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3cmsnltie.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfarbzib.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uiysjbdp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jbcuopeb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kopawvgh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yfsalesy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wwoawjok.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqdnnfpa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3awitugli.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hffdrmkn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwxkkjvg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjjnhpdy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzqxzrph.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xmnbeatj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xwjxmidj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kikuznot.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eabotppv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dlfkmtlj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3faxzmxcd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fuzfkqat.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qcqctmrl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3uazjwbfd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ktownrsi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3bshgszvt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kmntvdhv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jjqzpwpq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3oscjwlrv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ifdnejyh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ktzldeol.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jlewdcah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pejorfcl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mtwnlimv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uibavqkj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pqskhlum.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3gfohkznu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3typrdvxe.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qodzbdpz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gnnrdjxl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qsnbdxzz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3elvdhnub.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nrahyfbi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3brguulzu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3syatkkyl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3vomtmssv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlstlpxn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3odnskbnw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjwjnqlk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3njssqyly.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3pltjxetn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3glcwsduv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xgjbiiox.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jlgbcubm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vebkzrrd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3axgjtskr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mnfudswl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xmywsrvs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3oaylawhc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ymwkvads.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fehlqlwj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wdniisuv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kyfpnyci.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lstdjffv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nfntlwwt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tyotjixf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ywayyqis.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nwbczcqe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tluhafjz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mrddpiga.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3exixxjno.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dlclmyfh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3yvijwqye.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3upurhelu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdqcyzkj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vqmxbixd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzdctnhh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yhkfxzka.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gfldpvjp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3sgxnzeny.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3tgjjadtt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3obntbhwh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tmfqntso.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bnzesuas.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kippuzhb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yeiqmkfc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3fwudezyk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jewgdrvf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3gkihmeye.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3gsgrhrfe.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3uwakrbka.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qyxivgzf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yzbvyrkv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gywxtvim.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ssdqabqz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bdpeeert.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xvsjwpik.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xvjszwvk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ejrivkpo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3oxsbxqqa.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytnhpbae.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uibkcosp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zuwxeadn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3amputfvn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hvvmryln.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zpoyeqax.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vmzygpgm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3txwcfbcv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zjpziitl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mhkjplui.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kslcxyke.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wttohgpj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3tqpiftwb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wsbyrqmc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3sppvnpgo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfpwvexg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vwnidpji.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qndwppoc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3azjenhyy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ogxnwbxi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3smxnvaar.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yxjekyhp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3cfimllbh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zerolavu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bfvzopfz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3anxgmzsi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rllotxvq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3etfvnhfs.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhqmundp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kdavtxtf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdulxdbw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uklbxpqw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3fusrqtta.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pryvbsha.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eokzvakx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gapxezih.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zqudfvjv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qgudvmmr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3umihpcyb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nktzcqul.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ubtmwuvf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3plokokfx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wwgtufed.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mbdgenbt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ibekzkae.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xshjgmyf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cjyvqrad.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qiejwykx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xkeiwtrb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fraxpbwz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3htgrlxdb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3nafsukms.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fukjsosl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3txhfniyi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vhzonaiq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3eezwqmmk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gmkbjlyz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3yeuosoqv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3yvfogkkv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ofudnlec.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ljwnxcqf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ypabljgl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fpwmsxlq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3okohzkcm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kjbtzlvd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jvesszik.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kplbcgxm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3bvpohwyp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3znmofzho.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lspvyzng.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3doiwkpjt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ugsrkqfd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3irchqohn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xmpxbfod.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hozxgsnk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3woexjrwk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3jmmmsbse.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hyjolaio.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vbbezago.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyfsyral.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3mniquwzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfbocwca.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3bpahnltq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3kjrxffia.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoeendxm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddpibofl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwwgwfij.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uypxeoiu.html


<!-- 参考信息 -->