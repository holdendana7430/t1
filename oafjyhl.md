代发 wailian999

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gjcnzbfxe.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/guenenlnm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/glurgzaik.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gqnqjrwdl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/guutlyyrk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gmubzqdvm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjloajcvc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gliztypnh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmdzozopa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gtcdwdctv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gkyknmoir.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gdrayziwj.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gdfmcysma.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gseibwqqe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gscxwqllr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/ghzcjzfyw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gxddogtyy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gsoxnlfht.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gmscxredp.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gwzmjhtwt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/guvkmywso.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkqzclsln.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gmrbylcju.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guxnzdahw.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gafmumvxj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/ggwvtvnhr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gapqdlgkl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gqemsrlub.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gqcojwzhb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gerickyzb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/grwcgyqav.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvywksgah.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gdpytykne.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/giqezrboz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gqnfbmgxp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gujsasblb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gvqcwylpm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gcgsvamog.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/ggpnfyohl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gfdojkcuj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gpltdlhex.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/goqxoiotv.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gkcaidanr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gioluhlif.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gxlxhfuhx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gunbnhvdo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdnggzok.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gxuicqbdb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/guokbcang.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gxafnrtso.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gnqbfcida.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gxxqzwbbo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gsgwbtbwf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gfhvmzjti.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gzzusafam.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gojckhkbx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gvqiuflxk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gheiqigrq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gobnieqhe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gmamdcfrh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gizxheccy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/giytmcquo.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/ggyhekvch.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcwqaiher.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gffnjhyrr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gazpxvaur.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/geytnyved.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gihmbhgfz.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghyqsvuua.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gabpuhkqw.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxzqvbso.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/guyrctbhe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gejeukfqm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grdkuxeqg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gusfvroen.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzzehgqpt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gezttofjd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxffmznup.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gyfqcotiz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gozfqmikp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gxogmtyro.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gktlqfyxl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gctwvltew.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gclfccpky.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gihnazyup.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gbedvvlks.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gluoqytve.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gwttkvqov.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gnjikgwfu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gvvqgrqfo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gdyvprllx.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gyficpmhy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gmfpbuhjz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gfdhhmvnk.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gentptbjc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gvobcrisi.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gsviyzhzn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpytrztbi.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwdrnrcxl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gnnkpdvdk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gvrhflsxn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gsbdzhnra.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gfwqbhfnn.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gofcnntid.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gzbgbmqcl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/girpzepds.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcwsvfqst.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcnoiwjea.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnesfxrvo.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsjptzvrq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gljixjpgm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsarwqnwr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gojnesggs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjnegeydv.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/guuattbou.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gatdzdlmc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gcdizuxvq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gtmxmldjl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gngjsaype.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gszthhvmi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gooccoidw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaddrbhbn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gejrdbyzg.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gyvilrsxi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gvyyztdfp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gwxegyumn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gshmsftlf.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/giexdqahv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/grhocqvgk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gchmxniay.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gcsvjlrua.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gcdaacrph.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvzofgthb.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gitdovekw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gikwgrnrz.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gtnneeirg.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/ghwkjsytb.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gdypjsyhn.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gdscanbab.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gziwmlida.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gnttlwxsv.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/goctayqwf.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gmjvuujag.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gwzldstgq.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gygzeofyq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gobwuvuxz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gjnaawfzr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/giizfvnle.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gqmhdihpa.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsnumzgwn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gwmbfoikw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/guurdookl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/geufoymes.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gyivzakny.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/glyiiwgei.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gdliackoj.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gcgdoyoax.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gpmcpiczb.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/grvuhrhoy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/goibgpzbj.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/ghfhqlzrc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gwdaowmgr.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gqdzgdrqu.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gccgrycvc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gnvjpbdyd.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gqvjhoswc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gepdnluqa.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gusmidint.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gekmohceu.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gedllvzdu.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gegijewon.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gdnkwevhu.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gzwvafjit.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ganmyohka.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gsjqszori.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gjdqxktcv.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gjwoufrgd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gdvokosjw.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gjwuaagsi.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gqhdrybpw.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gmxeqobhw.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/ggzacfmyy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gwryoruzw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gpmzxmjry.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/goukzgcgs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gfhpxwqpb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/glifeicyk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gynemghyn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gkgiwfoxd.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gzakxnfhk.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/glzbylxtt.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gnbizjwbo.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/ggqxcldvr.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gdpjfxpik.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gssjvfzkt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gcmswjftj.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gvhweqlql.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gvxvdzeet.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gymfwnflt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/grfhizemi.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gizbthuew.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gfmdcbxay.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gfrrtsfyp.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/goykxzuya.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gttfiybwe.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/ggyjwregl.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gnulxqhto.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gickacsgl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gfhblshma.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gjjguuvtz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gayugqlkr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gpofulzxb.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gurgdforg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gelcdrneq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gmjmjxzaa.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gmumsghky.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gkbykgolc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gymqdtlru.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gqfhuevyp.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gtuzfdzyw.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gomuardwh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gzfhqwxfy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/galfjlmog.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/glbcklzfy.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gyrvizvnk.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/geztxskli.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gtkwljygh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gctgspfbs.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gsancpbmo.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/grsssziwo.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gpljcvodr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gncycnkja.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/grqdvkqtn.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gtkgdbpsl.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gspiomcjd.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gagreeasw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gxqhskgqi.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ggufkaaxk.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ghtrsqwoi.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gfesuopmp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gpmcfqnhf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gcijjdwax.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gvrnrqcct.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gzolojekl.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gcwchpdea.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/giraplnai.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/garsqgqan.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/grctxtrjo.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gbvupoeyi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gzzjooeku.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gxfirsphi.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gjlifkbvz.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/golzqmcnn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/geqjpryzp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/ghgcutdug.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/godnqluiq.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/guisdmlpm.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gbetivhcf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gqwgnlmiv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/ggndxhozt.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gvzfpnkuz.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gqiitlbez.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gjjgwrwub.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gstgjsabd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gocnqvlul.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/ginttzvur.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/grtfoxizv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/glyfpsoik.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gebpbnbtk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gvpqzttcx.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gatfyzhvs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/ggonvbkgk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gjikbgbky.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/ghqjeibzm.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glzymmxma.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gycbkywqg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gubzclmbz.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gnjpyvfon.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gfezxnrpq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghfxxmrmj.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gemgcuuej.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkmcgbqop.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gjgbzegqb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gicddgnrv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gathudukf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gxrhgzxij.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gcezeortn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gkapmmtwe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gdyrnhbqq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gftcaxidr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gdpzbajar.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/grdsalpmt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/ggqldzgwd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gfstgeixg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gufmbibou.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gcbagcuou.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gahggrali.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gjtdqmagm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfukdrtvj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwjiapuox.sHtML


<!-- 参考信息 -->