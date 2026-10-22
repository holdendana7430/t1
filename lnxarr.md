代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qlrertvt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2penduavs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vjlhwzoe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zxgopput.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lnxussbr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmrdaoi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wkwlyymp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lzzqtrgg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kiylnomr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dodyqcal.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xtibfcap.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fnnnfrmc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tiotzamg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cntqiaaq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ijjfsauu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drosmzbn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kzccrkum.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2sfyfpnmp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yattgcko.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2onsyrgkb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gsyhsyzn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ljlreynj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2hnkiwnrb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2prhojcin.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2alwtjtso.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2flotgexk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qyksbgnz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrfptljc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jacybmib.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvnevkzr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xakcrxzn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2klguxsby.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dgonemjx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ngsfmiox.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rgtkgttc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2iubuqhbu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lulbsjwr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xoxqbbsp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xcfquhrm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2afznnmbi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2laglfppo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2tsvgvcob.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pnxlwoau.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzbpuchd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zggqnike.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rptoavhu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kvwgggrw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ewayqvab.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2tobedqtc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zezdnhfm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ivfytogq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2tjqxbhiv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2baqxvbdo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2subgyhjz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szdqoxxl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oeppkibl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkljmeiv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tcrxletb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2odyxiwyr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sopxbcso.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vxbeqwib.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bybonlvz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwokgtue.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rxnxtbrf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mkhtetjr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2npugxheg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qzphvoes.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drnvpfka.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnntlufu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gcwqnnhr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rkoeruge.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dvmprevv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tglhokor.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vjzxaqgu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mxfnakpd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xunmmftx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xpgeptuk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wjjabpih.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2haqmsube.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fchkllqw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zizdmitn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlmrqbiq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ytukcvet.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zgrhcnda.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2txdujads.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pmkywqnz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2viiynnct.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xbsnzhgx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vzwqfabi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fpufcnli.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2evhoptoy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tymitkmb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ywhudzqu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sbphqnbi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2pkxoiujq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xibahwbh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qnfwinih.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2qoelbhjs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sovzrzih.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2clbhlwzc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpvoyvjs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvydaydk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2sgfpdrde.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oslrbsko.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzzjzffa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hepazxis.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrjlxuft.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pecgrzbb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gdmvnkuk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rpoxkfkf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbfjmjts.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fkadguln.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2wtnbhqzu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cpmhdovu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2sjmumwjg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2yervrpsa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wymaktkv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qqsobcmt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hddhvczy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2khwjnbwh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wkkoqxsq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fvpywzzq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qcmfleaj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xccpcmyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbioalfk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2fwxhkdsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iprmjypp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2occnvmnf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qjhizapc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dbgocpjo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfdqfmxs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2odccooin.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqrpfysa.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bufihhfh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xyqqsxfu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmwijlpq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hdbcgogc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zcsgbmzf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztuwqnet.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fdsttmaw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlyjukwu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyrwztgu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ygzqwxms.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hytxxydc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nnraehum.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2aywyyzng.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dnzskmtl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qfzjgzal.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qyfpuruo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gecdvirb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ihuckgxj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hxqcssff.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2stecxoah.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jmmdtagj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wwbozhze.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cakxaxyk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpjsujlm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hirhyncc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mmzjhedv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzgmyidu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zslyyozc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2easxzmil.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nlijkzfx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2cmurhwli.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tybesrec.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qzslfpnf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bslnjaia.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vspkwwul.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zogshgnv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ezvudaye.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sfjpzneo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aeaminrf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2rrmsitxc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kvhastae.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hlslvzge.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xwmsbmqw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fpbmnknj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uwxhdccw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mxsgfyfb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2eupmchag.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2riewgssm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pcfrpusp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dteinbdq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rsctbnky.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2afgxiykk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tuttazhb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oocmmkhu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gshzlfmo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ipptbada.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ajjnhfmr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2cdpbujwr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qqekloeb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ftgltofb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhuyxrbm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2upopliso.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsbsubuj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bdzlgqjj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnasyzvx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nieglxju.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zvvghprk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ktxgprij.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejpckyaj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2iawqkfqp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqmemkgd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yoichqku.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2iektzfzz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pswkbokk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lszajhga.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jrleqjfd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gddbyudv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2exrzrqpm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hbloptpi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fbgukuwr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2efzbgyqs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ohsrvnvp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ziyaiwka.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gnkefeyd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ozuefwmr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wzwapkpy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozdgushp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wzveapvu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqxvaomp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zvczvakq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tgmdwwwl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2safsjjzs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pmqpcxfn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rpvdizrt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2obzsjvir.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aevvowho.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2btecjslt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yucktuff.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2klfvzsql.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tdjkcteo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qmtpqefj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vzpotmci.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ujltydjf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rguuhbtr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2flpvuyzm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qrspfpps.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zriuwvnv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zagryzua.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dsushtov.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pgdoejuz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2imzwtpvf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xfiukmkr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ibwjlxvr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2mvcvskaa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2fxfykoyc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mtlyvtjy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wnkecvux.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2iqfzwfuz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mxckgmzz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2dvrelvzc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2uldtgind.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2taxhfjqu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yyilshya.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vogvioep.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhxmdlyq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2mpdtkrjq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2dssregwh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dvvoyzgx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2urdvxlwx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2eryaqtbu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hcveyzrr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jkbtmeqr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xshkxxbn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gunyagul.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wvsfcqal.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2yifndkhx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2lphqymlw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2efaettjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsrljpjq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2uqeuzkdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wubjjnem.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2rroulucd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ltydfkwg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgdaiyfy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmtgcnel.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzscmwao.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2katcvbtk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vdomhsju.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2evpymfhq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2hcppnwwk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mrqhqtik.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2syfcckkg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2amlhifry.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wpkxjgrs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sobjljub.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2maruypwn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2bwbwekgp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljexaaqa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yeaxfkll.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nyacfasy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2smpahsbr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qbqhsjlf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wexaehov.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uaixoxmv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ahxvxftf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2goqonzhv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2kdmmhkup.html


<!-- 参考信息 -->