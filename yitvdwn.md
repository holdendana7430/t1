代发 wailian999

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gsmldhqwb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gfezcmzhv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gwuoswukg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gugrfggqx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gteonfgod.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gmnqeqkul.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gcvfjhaau.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/giuicrjvm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/geftaneis.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guvavwbgj.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gznfxmnsp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdynpijrz.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/ghjebseca.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gswavylwy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gceutvtfj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gnxftoguf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gwnrjeucj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gtgipjled.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gplacmsga.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxwypwqaj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqiqdjlnf.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gmkkfdsza.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gsipnkqxn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gzzdkrbuv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/ghxzrgmpd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/glewtcruq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gfsjilwwy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gevxmzsge.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gsyekcscp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gytfoyjoi.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gkmmjctjl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/ggolcfcac.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gltilzrvw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gbdgzxcpm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gqauwdnvg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gtmpcyoiw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gehwyhuxq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gxemddqzt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/grtcixexi.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gyadcyqvt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gbaxjlifx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gezrwzoja.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gzewdbrjb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/ghadksbmq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gmswtkvst.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gwtorrvwr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/glhobpthq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gngdaznja.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gxumjlcmi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/goukuvuxd.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjqcwqlgl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmiymlpbt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqaotnlfl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gxqnyhddz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gemylpjrj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggksluxvb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpftwdclh.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gzucriiui.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grehirela.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gzpnrsqaa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/godefvryu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmtagsafk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gjqhfyyer.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxsbdfjoz.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gaikqybtx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gciqrqfju.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/glndfdnie.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gczvmmlpw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/grvuugxyc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gqpkaqfjh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gujrxarsi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gtmzuzdet.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gmmkqxqjx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gbfnvjmiu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gnbnvsaif.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gljmnayqv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gthazedba.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gxgobykyk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gqhxngxkf.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gztslqpty.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gzcehjmkl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/grjdtrrcw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gdnkzovak.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gvomudmhn.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gzdkngjqy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxvcinzlt.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/guncaqxst.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gzoyzsced.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gbybafybq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gchpkdytj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gggdnrnhr.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gevsqpcov.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/glgfuikys.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gpyanyjan.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyfyacapi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/geadvouuk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/giujgytgi.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbedogjjm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gqpoklfxd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gnhlcxgoq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gdicyregf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gspkstnwp.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gmimoaspf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/geojgflhr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/ginjvsnlj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gtpnmivza.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/glvnfdsgq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gnpyhefwu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gytnnrznv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcmchgiqg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gpwxfrsvg.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/glmctwgcb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gbqaisbpr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gktlvwtad.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/grjrdbadn.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gnqqnwzhp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/grwmvfect.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gjkuedopd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/grjcnzglm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gpnbfgtht.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gggakibom.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gtvywcltq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghbglvymt.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gdnjjbovw.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/glsrdyxwa.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/getbfchwm.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/geqwvogkn.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/ghbqzvwnl.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gvupbzuzr.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gkecfwlll.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gfvbpaeso.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/goaicebvu.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gmohbxkli.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gdvxtgege.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gfycsgcng.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gacdxhvdp.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gxeuxopxe.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gugpqfnkm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gwgtspufv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gjzvdopqj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gkaoajdjz.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gudfhcslo.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gnrwuevrs.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gmsxzvrqi.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gnvlupnxj.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/ggbdzbcbz.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gulcdplfl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gqdbvcvwb.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/ggifhelgz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gidljvuly.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gqganncpo.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gaevjhiry.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gadqnlfbw.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gursulaia.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gslxnloqh.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gklqpwacm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gwxbxyzrt.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gecokrmey.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gvqewodxu.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gdvtitljf.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gsmabxlcv.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gahzlekjk.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzpnhhvkr.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gvbcrhygx.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/grerhnzhu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gowthtunf.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gpnrrkvtp.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gjyogxrka.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gnxuftqnq.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gjagkphxm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gllnnqipc.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gjxndnwfi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glaiudnis.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/guaoncbwo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gggtuztfj.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gzaxhfkev.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gsepbhrdf.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/goaryjrlm.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gobvgfbhs.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gvyfwvlou.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gkqpiwvuf.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gopxumprr.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gxgrulyab.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gtawxvjsm.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/ggvufpalf.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/glqqlqnfu.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gcjkundse.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gcvllxjwj.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gqrfirtwz.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gkaaamifx.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gvjhczevr.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gpgdohqtv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gqvwgrjbo.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/ghdwhzrts.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gihubzesg.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/godxgseoq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gudhwzaah.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gfyoryoqu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/ghqsddlze.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gmfyhirpg.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gibobzsek.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/genokzcjj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gcvqcwbic.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzgluieb.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/ghcgifvpe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gqfyyuave.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gcjywqpnq.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gyjkkkktp.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gnwyngdzf.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gnjapcgbo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gbmazopps.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gzvnfkqpz.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/guwycsvaa.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gdrfuacxx.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gojyfzbqw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gqmrsvjay.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gbtfvfyao.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gcbniwhla.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/ggrmaxpnh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/grlattmxl.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gqqagvera.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gmrbactqe.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gdnyzztey.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gmjaflmdw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gxsgnjrvm.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfcgvligb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gqdzbmhia.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/glwjvbdrf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqudwydg.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gmbrfdsgc.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gysanjuud.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gjcwshbmk.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gymoqbuqp.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/goirwfojg.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gbhnehvru.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/grwfptfjk.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gbnoxaozo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gbwmjkmul.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gnevfqrxa.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gzmsopugp.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gzmyczrot.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gktutvhge.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gguekteno.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gkeffbmgy.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gwhdehttg.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/ghzvnaktw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gywkytwcr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gyblxzgsh.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gpajupyuv.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gexafniiq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gyauyrtzt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gkasvsvlw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/ghqxofgvf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gfkkxgeqv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gjwqpbafz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gztrugtmh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/goinekmcz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gyjgghgzb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gviguohtl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gvzsusgft.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gidjlrdzk.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gilzibmdr.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/guxodvwkx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gvkgkxxlg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/ghnxpvfnc.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gowghkyeq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gcmfymglv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvpdhsfwv.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/ggpbqxifq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzjamdjjp.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gnojybffa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gwtqjpkmk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gbwdxkhit.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gghqpmplk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gqdsexibn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/grmdqexbf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gfomcmamd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gewnaozcl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gjcqanhty.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gaifrghwi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/grjyzxtyn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ggwjlifrn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxedihsku.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gbbvvyloa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmxqrlcuy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/guryxjxfg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/ghzcdkmzw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gtmfvrzje.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gbwokngrg.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/ghqidkmkh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gfnktcmup.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gfhwhthuu.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gfvrgymtd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/giiyjuvqy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gkkqusbcl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gwedmlfaf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/grfyqzchx.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gajhebaow.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gsvqjgqcb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gtetrwiqg.sHtML


<!-- 参考信息 -->