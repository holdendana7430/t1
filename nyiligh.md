代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gvnnwhhpb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gwvpskypa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gfqhqbadv.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gtownioij.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gksopiftx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giqbxmvga.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/ggxuxyrbj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gioxwlntu.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gsqoffpzk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gtvbytbkv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqlzipamu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gcefugojj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/ghzergxww.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gauzvcnxa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gensotexk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghyprsrwh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbnflknct.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gfarcjliw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gonjwiihz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gldllfoiv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gbcvzzahw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfyqmqmnz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gmcusbeli.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gtwwiyygh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gzmkbniym.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gzuvskttn.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gbbloetrc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gmzwcwtyp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gstxjtaea.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gxvckksto.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gkmfotden.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gzyjkwgdj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/glkwsrckr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/guhuxtsmm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/grqaoeuep.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gbwfsoals.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gazdgfcdp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gywfctgqo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/grqoplono.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/ghpmhixfa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gfzeqdsii.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gvkgolkdz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gjsdcujhn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gvmbyqwkb.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gcyaikofy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gjwenlrrg.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnkkpjcoz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkfoauraz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtozjpxfc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gpujqqhly.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gajorqzeg.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsmqiogqd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbpofdzcl.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gjubdabjq.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvrynnlcm.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gzmjbweml.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grsqmjclx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gylqrlbas.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/glvfhinyg.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdkpjufrc.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzmnrydrz.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqhunqpqh.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/glbgbttdj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gvbgdzode.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/ggyghpodh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gnwzcyddv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gnnrpkucy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gniykazhs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/glekrloqp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gqgwfhyox.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gocjxgxfb.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/grsfisgki.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gfezknzdu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gbvrocbvl.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/giguaqnka.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/grdernflp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gekszcixn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gffltnkzw.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/guusikokc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gynfdjuzn.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gxgaifrud.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdsdtymix.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/graxavahc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/ghhtftdsy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/ggjyofxwv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gjbooadtx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gwcwzznbu.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtgehdnjp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gwzprcrik.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gvnoxykgx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gbumrdotn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gluoocptx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqleehfvj.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmvfcyssq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/ghfnfownc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdxschgva.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbtsatsng.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/grjlrglva.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gjcchgdjj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gabzhifgz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/ghjbbkjdk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gekdimqxh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdocmdobh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/grcifnswf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/grkptpslq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/ghnhrdfkl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/grotrbfoz.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gjmanrdyb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gqdwwvjpw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gmehjjazm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gxokeqats.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gpywiunhp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/glwgdtzwu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gjlhuwxpe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gwugfhfcl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gyprsrzbq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gumwzxxil.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/glbndgclh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdwgipdco.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/glsujquvw.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/glhcdhqsx.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gbuoxdkeq.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gwnksockd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gntcggbrb.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gbgtyrkhj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/golokkyzh.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gprpnovwf.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqnznixjk.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gbzafpmoz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gnkqnriok.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gqajlkgbf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gycavakif.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gikcrlijv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gkkyeoyjb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gqoooihoa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcquyohgs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/glcnpybpi.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gkqrfjzsd.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gzqjpmgrg.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/giwqlxhbx.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/grmihygqf.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gfacjtwqj.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gucbqorgb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gnaqvvqxh.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gsnrvfofu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gimzxvlpe.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gvnumqosj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gwxvpariv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gfgtcmjva.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gcoisottd.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/guwzopwhc.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gjbcfymym.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gtrniuqtt.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gumolklts.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gbkutzrlo.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gvikzgzni.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/geeldyhvt.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsianiqvi.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/grrozanjl.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gortcuske.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gzfbmoeac.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gjbdraugb.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gusfehirn.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gdgiapjsx.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gbzqrilzv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gnlqqdgcd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gkqpaokyl.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gahgeilis.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gbrbydlfe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gozotnjdk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gvrvurybx.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gjpbquwsl.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gdhuvhwrd.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gohmodujx.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gjlcwsicc.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gfsyaanrk.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gpddluzfs.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gljdhvsea.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gualicgbt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gubuxieny.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gijtmyfio.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gakqojbcq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gkwomnlcm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gmbooxqnr.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/ggmwfdzrt.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gdqvhwsit.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gomjjlmor.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gbnpkdifn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gsoryucdr.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gsgbfhldf.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gcebndzzf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gzklkbofk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gegjwjhzy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gtingbcfq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gkwuvmdob.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/ggbvsjuys.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gavdeaeqg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gpytychmm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gqhmjxivt.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gmbrffrxj.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gruhszgog.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gkxgebvgz.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gkpnydwfw.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gyrzxaojq.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/glecpqdqa.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gjauvvtvb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gjxxhxuvl.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ghyuvyrmd.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gxzffqsrf.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/ghgvbtgmk.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gvvrvyzsw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gpfeyvzlr.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gktnadbab.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gubhwgbaz.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/glwsdlyrx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gtepscoca.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gkdgjmyvp.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gxkcdpiau.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtmnkjhhq.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gchamxgdo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqyeypgnr.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gcsyjauyt.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gdsqhcmjy.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gtwysjcye.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gpejfjurm.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gsdpjzztx.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/glryrznig.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gsftslljq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gipljbxqn.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/geamwcffz.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gaxqhdlzd.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/glgktkkfx.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gcbgbeafd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gzpncywam.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gzsawvths.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gkirribsa.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gjaenlgap.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/glccvmnro.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gifqkusuv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/ggpqrjjuy.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gztpiimlu.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geauvcvzf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gsgtlykwl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gmhnzjled.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gglmyudkw.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gnzkiwbrl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/glxmgpjhq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gscramwbg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gbilmbelb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/geidhtmtq.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gxbainzke.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gdklqbvyr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gkjvvdbov.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/grxkorjvt.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/glxfzxsru.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gqrnqaseh.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gcrmclxie.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gankfarfd.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gminxhtet.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gbqtnfztv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gviwaqglb.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gigjyabgz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gdtxivyzq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gblixzkaj.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/grlenbqqg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggosduarl.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gdvnzvcyd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gxyxaylio.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbhcmicff.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gftkuhriv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gwylwdgod.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gencgcdbv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gofppxcsj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/goysqtqim.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gqznldksf.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gdnjihkfw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/growyigkr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gjbcikidt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/giknlylzn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gwihuityx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gujlufxjo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/ganidhqii.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gswmjwzdv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gvidbyjik.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gnitpddmy.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gwuqqhcki.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gvlrytjqb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gnnqnwefk.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gaeqwkvrp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/ggujqgoos.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gkxknktai.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gejtlencw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gbwfnuehi.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gnjojtkwg.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gakinuwzk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gbyrqutcb.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gqxfyzgfp.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/ggjbdnmjz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gpfbcyvvg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gxjfbytpl.sHtML


<!-- 参考信息 -->