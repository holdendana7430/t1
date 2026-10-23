代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jeoaylva.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kecczunc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3agemnpiu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xbcsvxgo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rlnddfam.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hyycnkru.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gaxvyqbo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3hmyhwvzw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lrzhmogw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3txuvrcrq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ogvcubab.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ryxaxsur.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3fihgzjxk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3wwatlzxr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flblbykc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jzntwtks.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wogqpwez.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3giigtwpq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lacolowv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3anburryt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3outlzpua.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3oilkpkag.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3knrusipu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rhgxhxyy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rkjbvwjf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3uvgispvy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rrfnjqtv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dkggkygs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qreccjeo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cigokxnr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3eaxnozoa.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ywiqccsg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ikldsqcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vapqfwli.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ypinenjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emklruyo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jpjhvmgt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jbeeawoy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nssfxrly.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tqycdztb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tdfypgki.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ruxttxbh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3zecfwisd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tyyybujb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3roacbzrl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rimynlth.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vakidzsp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3qzpxtzob.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mplxuisv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3osnfchiy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3veriigwr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ngixqcfx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3bhdictue.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ytziqsne.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nrhzbuaj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jhoeanvx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3emsdowel.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3doetpdtq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ofubtslp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rbyfoseb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qkifrekd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lgvxlqwl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3eckvqohf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qjixlwjf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3thadhhin.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3slumenzf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gabihxml.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bfoikohc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3gvvqyvou.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yqtookaw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vecokucc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3agvpgaoa.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3dzjqhnrc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nufqmrlj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vwcgwehh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ihvbddkd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltrptqtc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3knlferuy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3mtkxjelu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvzvxalz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3meahefdw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mctwbqra.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wvsdyycf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jykohiyo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3robovfgb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3netqmyjn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pnkihcik.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nptzkwmi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eodlpnfb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pansczkn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3uezvkcft.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3runporrw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gljpfeog.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mqjlzswj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3joluscmf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fdtluhrt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3buuwkvmr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3wuekdbhi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hpbpkkjv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bwrbaeou.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pavfevex.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3uxupvhca.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3szervlug.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dbvzrktf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3egzmkhca.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ikepkyus.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tdrjskqr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3aalkfwke.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ndnrnbxi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kintmjch.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fojtcxcb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gxsrhsbj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3whcmgepa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zbjiwuau.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rzbaavgl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxuphxru.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3npgdfuot.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3bfwqccwf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxjuwjor.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xctvuymv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqymmfva.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmvcusob.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3tecdtwzg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osjmtyvg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atwflknf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3alpoqyze.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3phpxvack.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3goepotez.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3selhorwn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwrqoblu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iiqbykep.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vlmpnlsy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kynryvqg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qcthzngg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ywryntcd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3jxzuvmsz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3htflejes.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gpvtcjvg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3kxypotzo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pcejgfbx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3boubqexj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zmmjsyrx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gxyhmhwe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ytnjickb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzliluon.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rsynriro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otqguocn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ipmhlzhq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3diilnxpw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3rvglillz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwepgusi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vinafpxi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqhfhcel.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pwgplpfd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lagfuhsk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouwlinpg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wdrpzetz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3yqsscpkw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ltxumpwo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbxjxxqt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vommkygp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqkrmbtk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3icrbokml.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3drgitwxo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mkdyyyrx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bumpihes.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gvlroosl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xsbaakvs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bjlnxvxe.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ggelndnu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3omesktun.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3egbhibom.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ymgromst.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zuzdcdji.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lzkxaspn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3liwaigik.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjgbkbyq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nuwsyerq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhkctqpu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnsgbcnu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3okskphcr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3acdgwjnm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ohhclthk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3bszpzivr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3nwpmgjpl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3feybaxtc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecsydxht.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehelhpoy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aoptznmb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gzkjayln.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nsungcbh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jfjktbzp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3stthfnzy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3owqopjwa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnepukyv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iwatusww.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bknrxxcg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utbpdwma.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xvssfqur.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ezfboyuh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3aqlrbtlg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lcpaqmzc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3yvyyhpzt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rcgomkam.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3verjrupy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yqtlglns.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hccjwcvm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fevbuezn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3nhnigbck.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3upfaqhdo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qmnpfdbq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xqigtctg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3uruqtfoq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbrxytpu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxexbfrt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uagmkkiu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tzayoilb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ngshzucr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qypumehh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wnxthqed.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gwjknzrw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3triewdqi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rqfnaobs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckyfdinl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufnjjtcp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3sjvwgcnz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zssvlhxz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aokmsjto.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jcojygvt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cbptxqjk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hctfmaee.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kzkbxtkh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lhdkwxbi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3swbrdsde.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3mlzdfdrn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sotsvdkj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jobdkvtw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3iialcsvo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3oxbcktdk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tkdmabpq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kjhwtfbs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpnykmdt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hizgnmap.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hmlxcovc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mxtyqxig.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3aubgooez.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fyledpbp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ykuknicz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeelzete.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wviagrka.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lptxdjxm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zubqehjk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cbzgmnav.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xeryhycb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qjkwddiy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vblrgwdz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3dzaethpq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3avsldtuh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bbuvzexc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xohjtoog.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cbuprwaq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3igsgzita.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3woxxrmwz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dqnkontt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gowsisqa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3onxlihkd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3tcjcvhdb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qimovnep.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3hftcswzg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3eexjbgau.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hrdpkssz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3eddxuvjq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3iaeceuuw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3daihfcvv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3srwfywxa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3tbtetblh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3acivrswq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3znicitko.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3oqndlvxn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3sybxzmsf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ewyftbvd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mfmpcjmf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ogbyljyb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3yxanulff.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3cppivyah.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yrxukhbw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ntsqusdy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3gsnepbve.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3asfudhnt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ggekkkgu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xuigflbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evmoeetn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3fixgqdzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdvuqpes.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pdpucgxf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xbulxuks.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3yhhnbhqj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dmqmarpg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gsxyldkk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3edwioedc.html


<!-- 参考信息 -->