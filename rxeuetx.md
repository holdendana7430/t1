代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gblljqqlc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/goxambcjs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gmwtkwqrm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/giuvovhdh.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/ghkxonlhp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gpoxvampi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/grzobudvw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gssfocqsl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gmyfdqnpy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/goqrenmch.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/glmnqfbcz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/geoquzyqr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/ggczsfzel.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqswhavzc.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gtwlzfpwu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmztqlfxk.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gmjuzyncp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gwoemvapp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gooksqcug.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gpilobaok.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/ggwegwjjo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkibeleru.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gqtrqykmy.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsivzgath.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gimkwnbjz.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/ggecgbhka.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/guqcylwpy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gighssppy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gnnzlyriq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqoceaqrd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/goucidxcg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/geaxepacp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gbddtgedw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gsyxucaet.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gwwjwycgp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gdvdntzsz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/grcdzwjes.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gchnxwxsq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/giemmdreo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gicwuczdb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gqxdfogeq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/goioimnfl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gncaupyvr.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gesaeintj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpxdzeymm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gbxwlvfpq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/ghhlupypy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gkmqyfnth.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/ghkuszgqq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gytqtmrui.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gnduoqycb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gzewlcytk.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gtwxhqspi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gautvyuxk.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggjodpexi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwidwhftq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzhrwnioz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gfmsmumfo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gxmoqtncl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grkbzmiku.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giynwjhqs.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gzrnfuxju.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsalpwlyj.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gtxryluyg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gofqhxioa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gddgrelwc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gnmgcnrvk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzjiryfpc.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbkhntaww.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghugddhsy.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/ghcfsipsh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdpbaugs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/geouwddhb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gnxfwpadj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/guvqibzsp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/ggkzokaqp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/grsvuzbhz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gztvzkdys.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gcnhlptaz.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gdgzemkly.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/grggirqim.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/ghxuoztxt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gvzbhyyov.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gmsieyqim.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gniljxivh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gmxrnripx.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gyeqymwqz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/grlvdoqvc.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gbsmzkblf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmnvkiiiy.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gnpidxqzv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gtzkqxwrw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gnkmliglj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gxjyohykt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gybztysoj.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnatawglb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gqpwcmpwp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gboiazpvy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glehsnpey.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gumpvmyyw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdfvlgpvc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmwanmmit.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gkctzhmxh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwonycwne.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyejubzyw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwqjwbrjw.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/giqckhlxq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gycxwedlo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/geejgllpe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gdgfrnejs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzimjhgnp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gfmrmyxey.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/ggeurlaih.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gmpdzszxn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gvdbmsbvz.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gstjifvpq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gtmertnvm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gjyklmida.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gpsevtlyb.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gotpratpl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gdaksmxzr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gdibcpmlo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gfwlwkzax.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gslrwpbub.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnlhditkw.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gbdgiaexm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvxzpvltf.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gmkkgfngq.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/guwsciclz.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gtwdugyhg.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/grnsttqnh.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/glofjwbbd.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gihgiobns.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gmndvsjhc.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gdfmqvfit.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/glsqbgaag.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gdjnrfdtb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gqwvvjwci.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gdmiaacug.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gxmucztpp.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gmbtoctms.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyvloajtk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gcpojofzb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gnwjlzlgw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gjmdsfyvh.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gmokatcmz.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gdphrtsnd.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gulupowei.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gkrrabxhj.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gsosfxgxz.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gaamibpzp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gbzescynj.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gqrmlexds.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gfdpkwfit.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gjdqmijcc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gudthaqxz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gbukqagyk.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gmueipfoh.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gpowiipne.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gvapexdch.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/ginbgbgss.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gchuxsaxe.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/goprhgrkq.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gmwqyplwf.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/grcdmykds.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/guvsbahwf.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gsgeyufgh.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gxvwuolow.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/govonzzkn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gcmvhmgba.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gfngdjvhp.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gszjixoff.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gcyvgzztb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/golkczqii.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gengyftii.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grbmpdjdi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmwdrotuc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gsllwblpj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/grwbsygih.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gcxeqojku.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gddyhrsuo.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gzzymnkpd.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gxwqncmys.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gttbvohav.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/glhmiolrr.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gvbtpvqte.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gicokvckm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gmpbiubmc.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gmkzdbmbm.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gffuqhpkm.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/ggivoznwr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gophtgqfk.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gnmsxcyrz.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gibcubrdd.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gcirewtca.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/goasfsmlz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gpnuujgiu.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gcmvzukoh.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gycvlqodm.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/glanoueot.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gdwexgnnh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gneqbsypn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gpshvxwrd.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/grgwtsjjb.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gbdqsxwhj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gxzcufbst.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gwawtftmg.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gkwaibkif.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/grqqfjxye.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gglxpmtep.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gqsijhlfm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/ggandwwva.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gmrpspfyf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/girhkrbfr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gfzhskuiv.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gmitmlxye.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gaafplcye.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/ggxeteohn.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gfznanlgx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gscyawmay.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gikfixtgg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvubcpenb.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gsgxlxwfv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gnxtrdkva.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gluuovnmg.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gbaeqpdzt.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/ghofqpmuh.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gctnjoysa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/geonlbwky.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gsvaqkexh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gnnpbfozu.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gnfluthno.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/guztfynqw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gkizyfzuf.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gmkerarfb.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gdpvutcri.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gefhyehgi.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gcvocctle.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ggflpdhrn.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gelkvxkze.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/grnfebtgx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gcqvtocks.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gwtaiczma.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gdyndgdrp.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gxfajramv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gltvtjkzr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/ghjfniwta.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/grggigvge.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/ghqhglngu.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gaqxtevih.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gwinbshjv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/ggsdstekc.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gkrwncrxf.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gfowlhkpd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gngdwvaqp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gisslstkt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gfdkpjifx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/ggdclxwul.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gvzihgpfp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gtqnktvph.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gjgqjweqv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/ghhwxtpiz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/ghfgrsfmp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gfpoxkbru.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gfgpekjmv.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghpttwjar.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gvincsjxf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/ggnplueqo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gufrtevnz.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gcdwyjkuh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gyjzwgsgr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grlhtuuyz.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gcaittisi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwllrzvjo.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/glgphscel.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/ggfzqjqpg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/grlvelrke.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gnsneeiya.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gkmzbagoy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gzucbhnqf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gkxmllmyk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gjivreeql.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gjzudebqd.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gfeqmffnb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gzouveaek.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gkqnfxrmz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/ghuryjcfs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gffbaqbzn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdtsosfod.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gldktrxzp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gfuslyszz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gtliaxaod.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gwgyhdyhf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gufxebavc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ggfzozrcc.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmgvrmaco.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gmusczljp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gbekimome.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/goapcamjq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gjacmeadf.sHtML


<!-- 参考信息 -->