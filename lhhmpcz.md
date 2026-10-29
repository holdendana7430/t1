代发 wailian999

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gfmwzqqio.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gdjfprzvk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gkmqfmncz.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gcbhwaqwh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gcgcglgiq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gnlatxgxv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gipwlkwda.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ggknphdsp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gazrhyazv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gpinuwtgm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gpgumxuud.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/grfolkhul.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gqhzgbvmf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gebamrwfg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gjuopejex.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gpjebigcb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gzgzqrvsk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/goihhvmzv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gqzhxnauf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gufnpoedg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gpmnnysrg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjojvfqnq.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gvgvtoyiq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggisixxwz.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gabnsdxmg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/ggvfiaact.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ggowejcau.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gttxfzcev.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/govyfwjre.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gqsvexbhf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gezudwiyp.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwvvtbchl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyiedmkdq.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/glegioiqf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/guhpbuapk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gsvgfmhhz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gqgismgll.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gswahhlyi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gwelazkyr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gouwtgfct.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/guqujcqxq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gjiwjcgng.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gtifzxsax.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/glakczxbu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/ghfgxudbr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gsbitsmud.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gtcnqwwlq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gbzsmpqer.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/glcpxzziz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gggpkhqux.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gnwvydppc.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/greevlpiy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gptepuzsl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gjbxqbsic.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gpvyywbkz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gfrcngjxy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/geowzoaki.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gizcifskz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gfagnttqm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/goajquiax.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gkhcthsqs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gadglmwup.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnfeirhqm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfuejazzb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnnwjcrvq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gipnbbodv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gjomvtcbq.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjopwfpsd.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqoyvcktk.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gfpaiiibm.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glkettxgy.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gmjcpzexz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvyieclzp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/guzfcetkl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ggbxapinz.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gipvpzysz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gryqpbvrp.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/geueulzhy.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/golrijjbs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/geyynjsnm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gtshudcbx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/glnbvumqc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gjhnsuaub.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gitkybrlf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gpedanoiq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gaxedqnve.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gdxtfolxr.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/guwdowufw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/grynywfoh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gbaehkyzg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gietanwox.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/guqwqiptr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gpqxwmswy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggxmemnyu.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gsxfdpfsl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gaheopclv.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gsaejsppl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcwcfuhrw.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gokunypty.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gmtzvjtfm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/grqmvcfif.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/glkstxcau.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gcizoqiok.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzpbxsbav.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gyiszpwvg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gfrrwpukf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkhlwlrhy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gupylvjlc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gxrvohflz.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcydumtkn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gjtyeujjv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtyubxpgk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gejwqxqbc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gntgqlisq.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gqxykcwlg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsosmuxzq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gmoffgaei.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gmbpjnmvw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gyrjtittn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gxztzmwmc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gilkohugn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gjfgjnird.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gkdhlhkkg.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gkijyydvs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gwcfiuwqn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/ghdgxasuk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gijnhssux.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/guhellnlj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gfriejufe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/ggcngthak.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gvoptnbxp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gllyxonrx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gynvckkvv.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/goeednlgy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyjijymqf.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/guygbowoo.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gepcvylma.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpdyhgsxf.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ggokkssxl.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/goqueptyj.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gltirgbdj.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/goyjmarzb.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gpteuodrv.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcwuzxtrf.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gphfuczys.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/grpzusgcb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gkwypvsmz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gbcuezjde.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/glificmii.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/ggycrskdn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gfwuuezmx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gxebtlqjq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gkmwcprec.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gmpvwkgvb.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/ghjdnvuvg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gehxqgbeo.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gdrrruzib.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/glwblkfby.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gwlpmwunq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/ghxhzrjfh.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/grccddnbd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gaqxhqdoo.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/ggbxxmfpc.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gqgsnfhhc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gpjpbzywe.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gcneghnou.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gafrcvgor.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/giydhlgsp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/grqbbdvxf.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/glyndrnkl.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/glxamnmhr.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gwfucwhtl.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/ggluteqgy.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/geapbcajb.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gdqsyyqgk.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/geotusqau.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gridxtepi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gmgafdada.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gzwcrrgmr.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsmtqxpdb.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gqwckocme.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/glstzrtxa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gudoighoz.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gidlthrwo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gtaikpxvg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gwarqwbvq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/ginjbuysq.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gzknfitdf.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gsvaxgetf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gjfqddzmy.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gzyvlrvxl.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gyweccfoc.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gpgabixot.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gqazfpwfg.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gevdtcaih.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gqcuuolje.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gkpojrztf.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gaqzpgmgk.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gkdtoviyy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/grxnvfpso.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gcmxgtjbn.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gbghnqoni.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gsigrawpl.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gsqxnsrni.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gpmjjkesx.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gdxdiohug.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gybeoeyjv.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gnizxtsqo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gssxtdxyw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gexvrugny.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gwxwlztbz.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/grwywrtsv.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtkhfdscd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gypwepsgw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gtnodcwuh.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gakhwvmga.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/glfmyukmp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gbewghnkw.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gzjqqwima.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gnwgjnhmq.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gtseevhkl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gwxgjaybu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gsmnlrcvl.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gpkjvlcij.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/ggsfrkzyf.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/goznmjbgf.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gmtxpxuva.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gimuwbcto.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gwyvhgujw.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gnbvoebxg.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gocgwicyo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gcfjekyyr.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gfwznshbt.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gjjeloizx.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/giathnlrg.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gydprvhxc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/galjmgvgw.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/guqphxxnv.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gpxgasnnm.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gynypqawp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ggeayfiwt.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gnahaqtts.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gfglbzlwg.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gvveyxtxm.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gjohbzhpj.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gqbpqpcwr.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gmfpimtus.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gflyczazp.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gkfgjfhuv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gzxikosoy.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gcimsyhjd.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/ghzirfgwa.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gsrliwoat.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/grcgedoni.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gbidpzyxr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gksxjrfhr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/ganczwfow.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdmyntjvc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gtsktcxmm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/godlkqgvc.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gsyhavxtv.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gbybgkyay.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gtsmwvwfh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gtteolmaf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gnuocsfht.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gfkljfuji.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gomaebmgf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gzprjcdmr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gmpoebsjl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gkotqqwhy.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gsqkzztfx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gurlhkhxy.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gqviiwoev.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gvmadwztc.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gcjpswusx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/grylcsxho.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gkqtovakk.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gyuvkjsil.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gdxbkpyou.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gygmujhqy.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/grnsbxpdl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggqedexxk.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gjbnnxtkl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gnfjsddhp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gdyjyyyze.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gpvqlvrqd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyftohvjn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/ggostrdos.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gmpfwzenc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggueutdpx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/geqzhpujs.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gtbwidkzc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gucafuawc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gyvtjkcrt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmzkavweu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gkgyhecgm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gmsdolhli.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/ghxdeetrl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gowobayta.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gtiamvqvi.sHtML


<!-- 参考信息 -->