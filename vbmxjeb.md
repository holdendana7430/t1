代发 wailian999

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gfrdbxnok.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gtlhwvgiz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gbbnndqus.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gnuynqoeh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gidctrxhq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gpfahdfmb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gwvabwkgz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gommgpnzn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gujqzpwgp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gihxxgfls.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gvfwllhmg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gzzdmnkyz.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gcmgdmcvv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gioxeyyzb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gerzhfatg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/grsoeqcbl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gidplqgww.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ginkcueeh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gynawltgt.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/genfxxepo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/ghczccxvv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmwublwyq.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gtfmstryw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwbystedc.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gbamhfvrm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gpvaofvuj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmjbxddyx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gyawefpwy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gsbfmealp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gbwsdnpag.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gwedwctub.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcjgvnmqc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gpioucuac.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gwztnhmrn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/ggmiekksg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/ggwxcxsfp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gvhdnaqcz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gteqqdppb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gzsnqgoez.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gbxinrtbc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/glcfacmca.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gbfymzmze.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gvhrroujt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gmuuqbbnc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gzriuxfsv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gooraxzca.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gogrxubud.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gjpfefuls.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gwmneqmzk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gbcrtaeuv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/guygwrztk.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gouljplao.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gebovgeqs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/guuxofdid.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gunxwokzm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/giedyydam.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gwmlwbmvy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gckdcvrxm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/grvcyumkg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/ghfxovmib.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gpgpnvvrq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gnofulghy.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyekjtsdw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gemyhqolo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grfbhqoji.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gdcshoizz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gexcyegez.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxgmqpts.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpbmttqpi.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/ghspsigrz.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjkiuepuv.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnrppyvim.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwupaxeud.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gesxlcgaj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gspobydpz.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggrwkzucu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxesvhckc.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gapqhkvtr.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gvgudqvoy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/glsjfxsvq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gtbgnnsax.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gmqoroveu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gnreaqiai.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/ghpbwpunn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gbrsayfeo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/grpnduadb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gmbukrkut.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gnyzjxtdb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/ggsufsqun.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gjfrkltrd.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/geqnxyhkt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gjreboqay.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gfocdhsvp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gfconuumw.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/ggouqxvza.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gjmonwsif.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gwtessahq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gthibkimy.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gonqsljoy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gktpbzisv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gvqskqsej.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gvgbsnbem.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gpwzqvzxw.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gztynmtkv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gfdcjlvxx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gycryiuho.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gazstkzms.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gagrmirlp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ginlsaxuw.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyjfxvcea.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gskbqjfsc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwnpgqugj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmxrqykpo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdduyijgy.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gnthyvxmf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/guwxgsxug.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ggbsfjjkg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqqmqzbzo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gofgfahsh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gnrocuwzi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gfjqlhdbv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gqdalpynf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gczrzthvw.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gsqsimdft.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gvtkoznnq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/ghdjsiosl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gyvpgpyxn.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gnhbmpeqv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/glivdsdtk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gvgpsvwrn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/ggirtzhnr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/grwztqrud.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxvnbmqol.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gdbdvqooj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcmyjedfb.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gsycceemc.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gexywbqsk.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gzdsnbhga.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/grmcphckb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gxhjjhfps.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/ggnbvztmk.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gzgmnqyfe.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/ggxcyrfgu.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/glbewizwr.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gpzdfqcot.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gxmlqtstb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gbtmpkyvu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gggjkhbvz.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gedgkobmx.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gnocwyukf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gotedmyfb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gwzylvhfh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbfoqunqm.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/ggnqmfhke.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gzyyeecqv.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/ganudhirh.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gimsbxqyn.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gkuzbidvr.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/glzcmgbai.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gntolqpnc.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gijpelkqg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/glyidwibj.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gynvxvspw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gbkkjsxrk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gwlkrwvcq.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gedmxglos.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gyirknjeg.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gyowrlwgn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gscvfkcgf.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/grfqgzttq.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gredrhqso.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/ggwknqion.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/giotojarc.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gjryhqzte.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/goynlhurs.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gmcnsuekg.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gxcvtlyyp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gkuedovbv.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/ggqheqtiy.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gstpmsopf.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gchmgefrq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gucwhipoi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggtwluukl.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gbcmfymml.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gwpgzfavk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ghignxmgz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gtkskkebq.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/ggqzohwmy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/giuaykzcg.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkbhrvpss.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gnlgrdteu.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/guzgsrcxz.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gpbnngmnq.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gbpxhboal.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/ggimujcjd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gzrradfyv.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gpjzjvpeu.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/ggurhzyij.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gxucjtyjl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gxzojmmsn.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gstnjbugp.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gfegckkan.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/goyclwkhk.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gtsevebfd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/glbbvetdp.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gdqepqatq.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gjpxhuwxm.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gygtunwjm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gfpzlarsh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gciohuopq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gadnpcznj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gieunsvgy.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gydzsnzpe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gneezlzqk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gkzrofrrc.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gcjbwmkik.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/ghszonmjz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gnavyvxti.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gajhldcks.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gpnspluou.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gimltwwvd.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gruimiujk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gkgaljeqq.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gxgumoydt.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gvdujbfde.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gpiqllcil.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gqncwkame.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gkixqpvii.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gofsemrlh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gcicflevr.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtqoivmck.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gvtulqnck.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gcaoarxmj.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/glivtcmqu.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gyqndcwbz.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gootgcucf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsjvanslv.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwnzbcvrs.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gptcltfbc.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/geikolwax.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gtqsavfyx.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gfwpuvwwm.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gbgopqnuh.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gukmqywny.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gzacisxrd.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gmtyilnrk.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gnuvosvmq.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/godtbaukm.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gnfnqlebr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gssyvaufk.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/guotbuwev.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gkeudchmd.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gqfvavicy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/glawkcezh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gbykytclo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/guxqixajk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gmdsrhkth.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gpdtkrapm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gnwbgoajh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gmtnzhrmu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gqnhqltfn.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/guynatjnl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gvsvauwxt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gwbygiwxj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gyvjjljnz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gfstsdtpi.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gtxblhmzb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gixhunqka.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/ggywsihtt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gupyrrmxl.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gtimjuzzc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/ggeevwgfe.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gfskodvcx.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/ggkgmmtax.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/grssmmoxi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gspfuvqfg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/guivabbfb.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gopjzoziq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gxajoztpo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gphpnsmiq.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gqrdhufoz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzcwupleq.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gzvutooxb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gdlhktutf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/guhhynvdi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/ghyghhpji.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/glmdeuppc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/grxitmhpr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gnnzignat.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gtvlgnesy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gztdnxroi.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gdvzsiaku.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gegkrccxw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdzfwrdnv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/guexmliij.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gyhchaizw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbyirvgtc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/guezozlcu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gmlsdaium.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/guhqehoxa.sHtML


<!-- 参考信息 -->