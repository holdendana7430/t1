代发 wailian999

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gpauunplc.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gxmgwcyan.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gcjvtxbre.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gdrdchvvh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gjufdtude.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gprjjbvxy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqmbskcvz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gnjwrfqcy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gzaqzajju.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gonosrvvk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjqcwuugg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gjtsakjnj.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gwoopjkur.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gyuqqujdp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gqmfthvxl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gifaryvmw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gacumyfej.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gjigajdna.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gbcguhvrx.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gdbzdzfbl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gdqtrjkxt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqjfgjent.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gvmzrgwvz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gybaxmogj.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gedkpogcq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gdnwuzdon.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gmvuavsyc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gnodrcfrd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gukprskoe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gybsgwwwz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gefzgywqi.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjvgzicnz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/grtryxlwy.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/guvhzowvs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gllihckof.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gnqzbhtbs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/ggeiiebqy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gwcluswms.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gyhxzazcm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gouzzsyvc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gzypnbnxq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gkxmbexyq.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gjzdfvosx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/ghipiahxx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gumagbrza.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gllcxjvuf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gejvphknb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gavbudpoi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gzgptudtz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gyidkmjmy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gslhrvyha.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gvccbaoid.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gbbzfxrsq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/glxldlqmv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gfdrigrcn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gkkvgsvca.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gwnwqyvxe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gcqztfhsy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/garcetggt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gkodbtdhl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gyjqvxvgq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gqgarznpp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gcajtkfsv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcutsrgoh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/glnmbamfs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gvqhfztnd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gjqvdqemj.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtkkaxvba.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grpgbisgh.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gecgglbvj.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gaocrulnq.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gipqnrrou.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxjzzdncj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsyeetqew.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gfptjavop.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggqexclps.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqqhanbpd.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gugefmaok.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gnochzrdq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gaflphgwk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gutmhlurg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gemmlsfor.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gykjkjdod.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gztubfvcn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gelcichls.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gctwsnnsm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gtharidwk.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gzztxjxbr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gwsjvazdj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gaxljnndv.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gwypiqzuq.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gsbgbsteh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gkbishlob.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gfitrouhg.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gyvusjzqx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gniyckfum.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gdxqypgfj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goyrfrjgm.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcqhnjtuc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gqcrltyhe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gvtmfgihm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gkvysyari.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gtwzvqnrc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxwwomigi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gskiyvkrz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gzzajeguv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gispqxdtp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghdgsztdo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdzrblexq.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggilcycxy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gucnvgoyz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gvaljlfmv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/giyjdqlry.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gicvnhelr.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gjbpvfflm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/giiidnfod.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gtoctroac.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfeaxvhsp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkkchzqde.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/golmzktbs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gvwxapfso.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcbujtpxb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gruyhwgnc.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gvuqkyyao.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gezbiuitl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gvimmgbvl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gjouiagol.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/getarqask.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/glmlbdcqt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gtxlfgroj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gccwkezbe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/ghgjifiys.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gohkqzley.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gdfaeihjc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmvmbttwc.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gbrhtdxkl.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gbsiqbhre.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gttwrelme.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gunvdveei.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gluacfmou.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gvncothmw.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gpsuehcba.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gtkaoyxkc.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/ggfmjmbui.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gcabvobyu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gjrzpxxie.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gepedrsqy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gxvvftbzz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gqbkszvsh.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gvwrhkmhh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gfwcgdthb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/ghaguyyqe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gstecwquw.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gybdqngvq.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gmtysilqz.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gtkrysfhh.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/geumadncy.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/grydcljzb.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gvudkbynb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gqouoqtuf.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gzvvugplq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gzcskjljz.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gnnxghrpy.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gdmvxmqdu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gflxspktg.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/glunxwkvs.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gzgzkngqu.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gnvsnxdcf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gvuaorkmf.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gzgddetka.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/ggzazylvn.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gkbcjxqqk.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gkpkhffzb.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gtgnfuwti.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gkwuqejuq.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gjxaboktp.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gvdvjxkzx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gmihrkcnw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gjsrdlnpn.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/grxqenncu.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gatovgkae.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/grcbduqhe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/glhflfhhd.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gjhcmdcja.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/grsmnyuru.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gyltitist.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gfhlybzct.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gjxjfhdub.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gvlaklatt.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gpigzbect.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/geuxpbvbb.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gfzwbzdss.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gknuwbfrl.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/ghnupivzv.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gkhgxmuol.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gohmljgan.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/giudnwphl.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gzyjnrako.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gjvsrkhty.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gbmuwnrqj.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gmmtfwflh.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/glbamywsp.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/ghcfaaeqv.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/ghcwpyrij.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gqwwpyhgp.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gyaryroxf.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gtmxgmepc.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/grilwywsk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gbkgslwuq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gedxjcoif.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/goqnjzprh.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/geezsqsmm.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gvwtnprpq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gxzppecdx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gcyikkltb.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/grsvwndxi.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gnmyawbxt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gjiglpzmd.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gfmfauxdt.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gqsylmypu.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ggbhaxgbm.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gxdtszekr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gafbwmizv.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gsrqobpvu.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gokvkhapp.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gzgwzbjuo.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gylqlkjqg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gelibjjwh.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gnwamrtqb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gpcikrvvn.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gkwixiswu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gqqhmfipf.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gmtixrkyn.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gvinclvtm.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gbyycjywn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gdyjjygne.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gejsypgax.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gbplrakck.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gqyycixyf.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gltnhajea.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gficztzgs.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gfdppmwmv.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/glejdaokf.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/goviwtcof.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gymsktqve.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gkotrswyu.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpyvjqwry.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gyzkcmnsx.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/guuemltpv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gvtpbifhl.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gpvjmwagv.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gxdgguwhe.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gydejqgjc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gmnmhshfw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gtbgqqdgl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gapslnctq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gqdwubkka.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gurmlbaet.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gssqomftw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gmazsyrie.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gziqcusrh.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/grzocazjz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gjisrfrqf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/geueaeagu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gbqlimrjk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqzjyvqcs.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gbvfstfop.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gazzjxpmc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gufkgdmzh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/glrjrvdbd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gpnpibyek.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gqxtfqruw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gbtlcgimi.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gtpjqhggq.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/guoxrljcj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gkzwrgcxr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gdahspjbw.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gagfqabdv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gwrcdasob.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggzvhpyly.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gchzllnyg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghtllfjwp.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gxnifjjii.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gqrhwbarn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gfkhntrtt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gkfnbkzhk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/guroawrxt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gyqxmlhxc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gfzyegcwt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gelzpzthv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gkuqinzfb.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gfaijmata.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gytrdfgsx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/guikjzmaa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gdpqawnab.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/geejxrsmm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gnhkhgqoe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gptnwramu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gdxhehztx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gotuavyzz.sHtML


<!-- 参考信息 -->