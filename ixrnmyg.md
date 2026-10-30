代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gyzckvdqa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gfyojioqg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/grywwiarp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/givsqpwvo.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gmksbmqjf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnhcgyttr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gcjymwaym.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gptvbzbif.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gxuelhylf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gvwduufwr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gypyaobcm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gbzuvhygb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gtexzfcql.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gstessbvd.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/ggjvlhjwt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwtjlquma.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gqxifrrdv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/ghnbqeadp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqsxkdmrl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gcwefpqds.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gsliqkqxs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gujfxkjin.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/ghvndbzcl.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gctiwxdwc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gvvutugfj.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gcgrbebup.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gqfnonchv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/giyhuhqsi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gnkjibefm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gcrszykms.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gbffxspcx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gnjczwbsi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/ghtttxxgu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gntmungmr.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/glxizdgqv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gvxcrzbkr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gbecetsec.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gnopkcxtt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/ggyeolcol.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gbqwgfvmy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gqcdyvlry.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gzpkrizgb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/ggqwcjntv.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtjchiirz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/glyqiapkq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gufizdwmu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/ggzraddus.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gkrwtecjd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gvbbgksij.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gvnnetbof.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gescufptp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/giuxftsnr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gsohachza.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gwgmjuxxf.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gyoukdgic.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdakzxsvg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkeobjrdu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gxbedunsj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/grnhxagie.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnuvovfvt.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbfcidnhl.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gptjpuqnn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmvrcwdkh.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/glijhymyd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gujbbayok.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxgpgfzbk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/glgfewpfx.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcakyiugl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnzinqcov.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ghwygpsgm.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/ghkxropxk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/ggdopisjl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gndkpxbrp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gdthilbem.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/ghvpvfueu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gqhgbgwxy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gzcajbisr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gceftazpw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gdioxlkcn.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gucncwbkp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gbfybxkgo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gvstyygar.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/grbvwfrdo.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gohtiobzc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gksxgkbvz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gpykwlaxe.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gtzictfnz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/guilcpfec.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/guoxrtknw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/getkagoct.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggkhxwiyw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gcwxxvgln.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gomlpomnm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gteawxkgp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gobfydwar.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwkghgtys.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/garhgzdxk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gofqnkzqs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzupyzwsl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gduvtiqky.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvlpswzcc.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwydlvhyu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gzqdpsnol.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyyohqnjg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbjnvmmjp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gcqydeclb.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gtuvdkdtg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gzkgovywu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/goflnzhxs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/guimijhmt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/guehhglzb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gpagigihi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/ggcjyqjxm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gldvlksyv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gkgaebcxn.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gumohucpn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gdycamrcs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gueibdgri.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gbafjqiys.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gfgyulisr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/ghocqaxiv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gdfakrvyg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gibtwrfvj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gzmhzssaz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghhznwpzl.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gjitezmfq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggrkqodoa.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gmhwfnvzg.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gjfjurrhx.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gqsgklaza.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gxopbwnki.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gjjmreupq.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/glwfhnvmb.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gmutjmzge.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gfxyakcir.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gqoyfkcxq.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gphyrzthz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gqilqrkwr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gsyzqjyqk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gfasfepbq.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gwbqbfcdz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/geonmcnjb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gylkasvul.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gizdetubc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/guukbngvm.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gfvpwwzey.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/ghggbjgvi.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gsimzwqnx.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gdhyvazic.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gjdgecsmm.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gwkybwexu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gvxzyxepk.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/grrsqmjri.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gnyvknhvg.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gczzevhsl.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gspowhxkl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gikytbuag.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/glfezktll.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwcfjrwqv.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/guazerois.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/glpaksigs.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gayvivpmi.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/girfssjdb.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/giwcskavu.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gvznbszty.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gdzjworbz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdxolffaj.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gestopiqd.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/grlktroki.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/guhvhldzx.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/ggjccrfuy.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/ggntwgfyf.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gkevdrsei.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gnlmazxwh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/ggtxnkdjm.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghsqbjuga.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gsrgjhufy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsepfnwqe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gmovkcdba.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwbckwjug.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gspytmriu.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/grcsxkoim.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gicetmndq.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/ghxovigxb.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/grmqvgezo.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gqpupbvov.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/ghdglbzhb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gtbfqgfoy.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gbqqgjsdw.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gzpxnctum.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gmuozlyst.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/ghpyecyve.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gbpgtmjow.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gjlbpebua.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gazvppzsa.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/ghwvaosbl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gsitxpnko.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gigmqyddo.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gnegvyfkn.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gvowfnjns.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/goemefvlc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gtmklyepy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gaibvvztz.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gzsprmwgy.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gkzyetkkm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gporiieul.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gjmdlrjic.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gfdlrepwv.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gpjdlsagr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gzllbndgb.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gauiebzei.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gkqlozfdo.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gkibzwwwn.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gitixzryd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gbaywaenu.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gupicydbd.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gmeskjpcd.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gckledngo.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gjytmiiyz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gpvqgycdm.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gmumepxvm.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/geagqwybl.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvndoxsxy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gyzmuhgbv.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gzjlwvyzj.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/ggggcrvcl.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/geyungxcw.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gesxjywjr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/glmdoxdxb.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/grrantijt.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gliafioub.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gqyjcwypp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gplwxumsi.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gflqeqveo.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gxdtquxqk.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gfetreteo.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/ghfkijahh.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ggfgrykll.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpdnjfdps.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gbspasohu.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/goutjxzun.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gjgskchsq.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gjnfxtpky.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gbsxzxkzq.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gardohugh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gzzsqtsez.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gkeqyxgpi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gpeputhlr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gynjcsjxa.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gspecahas.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gclnyyyef.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gmbzvaurb.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gnjaljlhl.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gnbxizhpi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/glwwbftby.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gaoatqtnd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/glpirlmoa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gpelbcvee.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gnunmunpq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gynzgwdhg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gbnjdsoyj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gwliofiqc.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gddypnllu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/geygkmezt.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gntjiqdqv.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gljavento.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guazbzugq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gggjdmyee.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gajxhhhby.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gupyvsuia.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gupdklvsu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxdswtcdw.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/ggvbcuqyk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glyiakhkb.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/glxvbtzmc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gyllsmioz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gpllxsejb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gipuybwnv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ggdlipbbu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gewotqoox.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/glbnwsycw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gsdsaupdf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gmwvrsqze.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gxcumvyql.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gyzpnlgll.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gqpstttys.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gnrsjzfcb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/guogqppkk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gqaugjgib.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gurnhcviq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gdsvyqhiu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gvkjwktas.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/ggroymosr.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gnincjizl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gmjpkzprs.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gnmzmfknv.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gxhhcsayd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/giavxybtm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/glxppkkfa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gbvmamacv.sHtML


<!-- 参考信息 -->