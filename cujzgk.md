代发 wailian999

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yqyhssqi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3hfmfvute.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jahbclic.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ypvcohku.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3igdeylfi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3noxgnfwb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3kthmrbkq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mzmmzfof.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdtvxvrv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3hktqkewq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjxwujiu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qvatywjq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3rssrvyuw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xoooyvgq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gragauln.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3legrliao.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gbqqcmys.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gidennam.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3opxommrp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zvpwhdmz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vteyizur.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xoyzxkgy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pwrxsxfj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bjxermeo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cfhuulne.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qdsykklc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bvtyuwyd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ogssvbhk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cfzkevet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgtfplfc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3jrriexwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifpclwga.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzkeceke.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3waduincw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iehzjuql.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gwufhlqo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3potiexos.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ydpsxeor.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rvzmzyth.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tnlqamki.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eqjyqivm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ephqowno.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3aqmmworj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tafxvhcl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kjqjcrne.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fgjhkpiu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmngrji.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kxzvbxxv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rpnufhbj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3axqydhep.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3byffmqfw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qwughucn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3odonnuwy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wwocnrhu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lppjnqem.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mglathrk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3frdinrzl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3twkyrago.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lgydxkao.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3blnrerva.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3welipmop.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ugtisfbg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3quiqrfwt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cgzabefe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bguoyirt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cigbhall.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3wdsupdxz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3frlyhvxd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3swiaupnv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mbcqksru.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xpblhpxq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxtsbfjp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tnyyyyla.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xuhkjsvl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ytgzcapt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ququuldx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbtitubq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvthzspi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ximmdbxe.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mmujfbck.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kkumuazu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvwlwiss.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iytjjsoo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mvsdfbji.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nsdfgozv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bdyfweed.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bhwkmnmo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jozrjwln.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3exjzscti.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3penctrln.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hkxobomm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hxmlnnmr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pyqcmbdf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3bbiyjcej.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ejeilahb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xvolyuyh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3tqflosoy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3uxmpcuxv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cbrwfpmh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bahuanas.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oyuxvkst.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3dqtjavdq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wvjacktf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3awnnzycr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3dwandkjn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcezobjg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wkaycrew.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vcyzneeq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wduixpha.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3klfeedds.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lcvvyxwu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hkzayhis.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dxijelfh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3unxivjgy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkjtxcac.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3baxhmrxs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcofseop.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ocpwuqzx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kekbqmak.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frjaeeyk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzownuop.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3amuqhsdv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ntuqmorr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lffexlzd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xglavnub.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jcefckve.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmmcawwx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dcllagbt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ulsxhxyj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3weeeftvp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dokpibbd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mulbjnzp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ovryvetm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3hyxjdiiw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ctfuyfyy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3fouccikd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mhxcbzki.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jzpxhwij.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pxkhnlvx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rfwbfbnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olqakshp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gsqtwhrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmrzmvnv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mseclxji.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bzzvyxnj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3prtjnzqc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3omebyqdt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dnsqcunu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zgxqwxgn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3kjgwfvnp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yepbdivt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgwxyugo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ypqmarcx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xhveydeh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jupifzrd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ljqfpfmf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3egkbpiuc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpzmkwae.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3sstwvleq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ebrcbljq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pgblxohf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rvaxbdjv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gidnithw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3neygljeu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sngeoezd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3utlewpgu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dhaimufm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rrhsssaj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cqxdcbaf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wcqaljqz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lieldnue.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pjudjtpb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cekstkki.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mcigqtnx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ivphclvg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3frhfmmul.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xrycmyar.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nexhevva.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tmhadyor.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3blyzukry.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fjhyzsmh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqatxujp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjzgrbtn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnsbsisx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nlctnhrj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hiituzud.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dqnmhpvu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xunqwgwb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rlrkzbyq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3gnfiyaht.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3votjdskc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3arsuefti.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3foqdlhey.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gurdczxr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3lrfzqsjc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3smuenqps.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3izejgish.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3gwjkgctl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3llvdqynx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hqsofxgl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jndkumus.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uglxnnmc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cqyhtzgz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xvyqiqat.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3exsovxpp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3stzjsaib.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fmoeqseu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3lbictwic.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uevobqxt.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3slubzajr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pcjgiclk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3llbvzztg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ejbgljii.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3feclknqm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3crmzpstu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fyexcpcr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vwqvhbjp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3recbgsyb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rokebefl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrlwmskr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3moclkokh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xvfgvbhf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3eyxhqaqr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mqmxdtak.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qilfukbt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zyvkygfd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kurlcccq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ozftfvnq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kxnzludq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rgebwudu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gbdebplr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fkehlcfk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3djmpmwed.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3swlegkdw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tskabkvk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ttuproza.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaahkedg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bqbtgwve.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ddtadhei.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rertqzih.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3owwqyzmu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqclhgot.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pmzwhtax.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hgsdetle.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrobxiqe.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bplpkmri.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3haasiqvj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3saqrucrx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jdbrywyt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tpyfdmqv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vjmfplis.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tpbysfht.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cdffgfqb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3saawswsc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lhnuompb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ytywfipi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vlqhoyhx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3bjhkftns.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vdwegvte.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yxuvnrnc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nimhdkod.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mqbexzbl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3skryrxcu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3zxyjdbkp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vgpiwtsl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3coicwsdw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3oinghozx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3pnwesadg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ppaauyso.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3fwlzibgo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3oafiiwye.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrotqshc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3uvfauwyu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bqqkuoto.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3przyqiwh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3dveejxxs.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vhtkdmla.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jntyxwjj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dyqpsklu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hcbdjzcj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qgynocnq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3arfymxfy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zcapmszt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kvevsugh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cwvmpqel.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3yelpdjmj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cbdydgmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3liebudhb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ymhvoqvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psuytlsm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3cyhqkhqb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3upatpfss.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbzqbfmi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tohrcdcq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jpcyfgrq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dxvmjtro.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3odpzakeh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3dczyakfy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3cspvvlid.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rfwgkovl.html


<!-- 参考信息 -->