代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3gjjmpvel.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tkgvwccl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hvvpxqop.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mbqowjqj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3mqtdbizc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dggglcxy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vynziewv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ypvdwafi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ainxyzcd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3gdoxxkkb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kvkmtfyx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3gviigbzf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jqntifji.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3squuitin.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rlzqgedr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yyyploez.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3chshudkn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ivzxgiox.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gfltylco.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gfvizjci.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qabvvkdz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xmqbzdde.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ofbpcqgt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dgkuqmij.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xntnpljs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dcwkuavb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3tofnjcip.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oezpfdgw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hvqaymjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddeluekd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gbstkvab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrdjzsef.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3spjbvndd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3blvabwbb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sgzkispy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qtmecwse.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mqfxbhmn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ssqylyjg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qeioouvs.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dajlkzqv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yxqkzgrb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jxgzladi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gzhlcver.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rzhqayyu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ciquvxkn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkdwuzis.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aydywbdf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3mgiuygdp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3odqanbbx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hffnixba.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3untpjywz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fogaygxb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fsrgemxb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rynoxgsb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qbasocqa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lbtgrrwa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dhydthoy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vcyefgdw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3olxougww.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3dgnzwidi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nxbztzmh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3buufmklu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3drrfghkq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ifspmlaa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3sybyhwlb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zuuutsnv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zovvzdph.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xkvkbsom.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sbvpfqfj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lcwfvvrm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mdptyvwl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mutmasad.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stlefogo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vfczzwso.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yqislmmh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdkpgqeu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwraqmcp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fedlmrkg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3goqznhbx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wtbiwmik.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lvxpwtpj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fuajefjj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ewcefijc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpnoaxuh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oitrxffn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fpnbsams.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3gnkaijtd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jdmmwxlp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wrllfnsv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cxnnhqta.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qsxlxnqq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vlgsgngo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vjnggvhq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ujqegynb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qcgackuj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xmudyqgu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nmqjsrav.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjejxosk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xbsvvsus.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3eehcznzc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3keudsfyx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3okedfahe.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sjpxrrni.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zqwgnxia.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lnvwmwir.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aifhendf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jysmdrrw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qqbjwckg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dgugruix.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gxnfphyt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bpfulkyx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ygaawsgw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ocantudm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3cvsiipcm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xoxwdtsw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mdwnnpdq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqmagzdc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqntwhly.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3hngrvfgb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dcqchoyk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pporrvgo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdzplnck.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxygdxun.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3musptcct.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jyqdtder.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nlzxtfqt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlusjxvm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bgiuaymt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rcfztnqt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aujtdrhg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ljchnvad.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3liirbotg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3aplhemkm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3vtogodya.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3cbwgpyul.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3qyosrwdp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3gqxsrapn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zrnyqovt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vimigcio.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xladzweh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzfnaxnm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3igkprifk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjqzaylg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3luqmwyam.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3japnqtwn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3freuinlx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pwtgbpoj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxsmjgkv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddchumwy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3dlzrxhid.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vpymvfmb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gdgqovvf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vmvxoopx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mjuzigbc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtsnswgo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unsplbhd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufnnpugu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bfcjownp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dchbltdn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3btvshcoq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rtikinur.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3txkbsqxy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vpbalbhp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bqoqnzii.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rnqumyvs.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xqenvopj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3epgjkvog.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3miwaojln.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yntuexni.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dgzxfspz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3onkodahf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lcymheyx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xsqtfrgi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oygbtfpi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thihxwru.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3edcjogdd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3blzjffpf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cbtsdoor.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nksqstdz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3llbhytgq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mwdorjly.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzahsdul.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pzlgphxe.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dfdxhlzp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xelcvgby.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3brkfancp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bvfktyug.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hmiqlmjs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bqltybgo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wumklfnq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hivzifyv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkmfrsxr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zicpawjc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hsilfnxn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3oznazbki.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3blquiglp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rwymqtmy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hmduotsg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3yqbmyboz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aujtkpbx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pylxazoc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fkplqlol.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tzbdkaor.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xgxdwxhv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gxbyfdmw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3sootzvez.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3huhtqvxi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kricofiu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcuxziwm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyuhrmje.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruimkpqu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3igcnvkek.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fwtrrcmn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3jmwuszgj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3stssqxfk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vdalvpzz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qcqwnjyg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3juvacors.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3pdvqckys.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3cyjsanqr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3bctphqav.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3anlozvzt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3nromzcrt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnnvejjl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3erdydkyu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3csjddhgy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wemdhdom.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3yptnhneb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kvtexlhi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mcteedoc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ukurbnrq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3isvqvxbu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3lejfvtej.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3aollglus.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nddglojt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wntxjkqy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qprkkoej.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fctuplrh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edssvoeu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bdiisody.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3orqlrdsk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3acbdxsrg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eqabvsqx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qiazerxf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqdscwwb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lemjzjop.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixznmxst.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crrvdrkc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yereaqin.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwsdzade.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qqazcvmp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ydjeslxo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3igxylpdz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yqtomauh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ojkikzyz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bzphyomg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3blxogspb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3twdtmdyt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ttdjmkui.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fgamqhux.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3lpukodtl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3kfqgzoni.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3uhztttmh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vsnfwzcs.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3dizbhfqz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ikgpuqny.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3oekltgdg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jwgndmyh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3cjzjkbyz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zssjyamj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ebczgldi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hrxldaep.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vjsofiss.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3azyjhgzk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qevmmhdi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3dgsvdkwv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xugkuzws.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jwmrdaoi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3cmsrfoml.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xrhcokul.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xgtnobhq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lqdbsryl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gbororjp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3bnhiguzm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rhldnjoo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3nphnlfpu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nzqbgkri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjrwxrav.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uylfogxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmpwaftr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3wvjrbnux.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3wznyocvu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgwshhuq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uusyemua.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjhuqtxr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xczplrhy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3mpzpeevp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bbnxmykd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3snjdpbaq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kwysncsj.html


<!-- 参考信息 -->