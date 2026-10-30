代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gshkxuqvh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gqhplrguk.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gbxxwheam.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gnarkwjxw.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gdyjxxazk.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gmoxhftsi.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/grnqangns.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gjfnoocvo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gbalybqvp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/glbjnemld.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/ghgwqztzd.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/ghmishuaj.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gpvqxvyue.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/guoisnqav.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/grfovvjor.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gsuzwxtxw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gpbzppntb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gbmwbornt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/golxnyztb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gulepryjd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gqkmzwucz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gaowhptnk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzxyemjkl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gofwxeiav.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gexwpeoew.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/ghscnbfqr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gztczzscv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gmpbrcedp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gxbrfieqr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gsqhvzqqi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gmlrvvqln.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gfrglmkcb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gohflwfha.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbhjmsdmi.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gzomlfvie.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gabdeuvcq.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gdfkmzwdc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gfztlhnti.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gokkctsey.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/ghbkyyphv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gurnrodol.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnfruvdat.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/govizjfyv.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gheztlfzo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdxxlmbxx.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gdawgbwix.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/glbzrvddj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gmizglsdl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/guyuevysr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gquidvrpw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/ghczjvhgd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gvlnihhcs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gialzgayx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/galtfrsdh.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gcdkmfdsw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gjtgmbzff.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gyutkigqn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gmvdseiwk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gitqqvjar.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gfmngorzj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gtfuseijb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gifknomkc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gmbacftdd.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gkfuvpbcw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gbsxoarll.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gkrwoblmu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/guwbxxapw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/geoslfnqb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gnkpmdyff.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gdxzgznid.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gyuenjzpm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/geidlpfku.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gvqhlyphx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gnxttmyyk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gharzdwkl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtzbvhmye.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpuhvcwjq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/goeufeoio.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/ghxdonjzy.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gomjbkhlz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtagqawiu.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gkezlitya.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grxyhgwyq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gohmrbmsf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmmyuwelk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grqhdadvb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gsopleoyc.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqyqjkkyw.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjpasfuma.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gcsrssagv.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gtfvhycae.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzuxjuvea.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gvjwciltl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gitfjrucu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gogwfevtv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gqtggnpcm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gitmkcewj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/grjpehmjo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gvocdezzr.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gjxkferui.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gvqbhzjky.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gvdmsguhp.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/grutvlgak.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gdoytfhhx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gavipreft.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gbeyxkbmj.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gclclvtme.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gicskehbg.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gqquwjpwe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyafxnnfa.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gihugadxt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gnvtlevaf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gbtpaxikp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdaintycs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gzsbaihzw.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtncjqsbf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gfszxvqao.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/ggoudazuy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbgxuzgog.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmlpflmem.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gxzptvayi.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glhqilwhr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gxcacgogm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdpyhivva.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/geevklpxe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gtmzljzkh.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gmmtbdmej.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzmnwiqwb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gaagkrank.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gifyricte.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gvxthaimr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gayusmjrk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gopgwjini.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gkxdmwfii.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gmxskddss.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gnfswkhjn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/guxirtnls.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/giiwillwb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gsesluedo.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gzrfqnlcm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gqsbdzayh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gehsxhulk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gomzinwdw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gajlhplmx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghitqgpld.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gvbxiaycg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gccqhornp.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gwyfpuvsm.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gvjiarzno.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gbwuikccz.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gusyzvvaj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gurvomlnz.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gitpkmrun.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gmvbfpuuj.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gbcxxmwti.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gjidfnvzx.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gbtmpqmcf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gwofzpuhk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/ggfbjrwqe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/golkutewh.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gwxldxxym.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gaylahtin.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/grvobwvvo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gtwmmsygv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gfpqofymr.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gahiewpdx.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gescqexov.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/glvhqaqgg.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/glwejbunt.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gwcigzgfe.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gzkheemer.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/ggbgcdvyd.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gmkmkqgkn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gbtmlzewp.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gdzlpdriw.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gwqeeqcpi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gdjqdjqwq.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gyfqrmqfe.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gmyoibjxu.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gvnoofujx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gnfztxpnl.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/ghxxdgpoh.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gulsrrqwx.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gprbousep.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gleqgdped.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gcbwfrggs.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnptfyxbg.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gkurseomc.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gzwjmqsum.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gkwocnjzi.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/ghtetkxfd.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gytgmasnz.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gtabrvmmc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gluqfnbay.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gtojbfxta.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gzvyalmpg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gaccxhzdm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gdkhpxzkl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gcafqdxqn.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gtqyrtuqs.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/guwmxzuvv.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gabrzmhld.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gdhxpyvkh.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpflkjvpr.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gutcrbqsv.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gtegnzaul.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gxadmjpvz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gpsacqfrx.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/grqdlvpfl.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/ghfvhtqvk.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gtxzgvvpa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gqpeusxrv.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gtsrdtdwt.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyqfdvlkl.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gtigbbowt.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gjxfamvzi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gebpsaxkr.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gohwqmlgi.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gnpmoynif.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gjwxqvdop.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gcptngmua.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gamvyzhlm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gmjwozqlv.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gkgqnedit.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmjfdwpvm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gqkylgzta.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gqvdowblq.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gsyeykdfk.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gaygbvjuc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gozybelgc.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gpejuxpdz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gbdmcrqqu.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gsfrweswx.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gdqjchmdc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gliagfykq.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gaijgtecf.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/glghzzdvq.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gjavgrzxo.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gqtrbyuvi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gdohkeejg.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gnkpvknun.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gpzcmsbid.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gzcxfxfap.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gwbcqxtgi.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gujudelqf.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/giyrsbcwh.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gxqjcnrsw.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/grjfmhxrl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gqwvozxpe.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gdbfhkjnu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gneuqrztd.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gunlwknoi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gyzkdtaop.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gqzaqukui.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gbwskmnin.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gnvgqvmon.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/ghgxxaxmb.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gvhbadvbo.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/grxbfspha.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/geopeaifw.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/grjodzfsp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/grrlnbsgv.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gpffrtqqo.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gptzyaays.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/glebwmwaw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gggyjyzdq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gtxwmajlf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gfklestwu.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/ggetdyvot.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gsbwyicup.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gspdbynug.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/giudfbipd.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gtcvzkiwk.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gayrqcwsv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gvvtbmbki.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gsmgnzrct.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gpptkqakf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gwhuwqkbs.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gueyblpxe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gzzoytkzt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gjrkicdlj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzfkeieri.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gsdefruun.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gfztuozpz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gtfdpiwyp.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/glbvzmjoo.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gcakxlxqd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gwwupevna.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/ghuehmgai.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gcnbfdkxg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gzkyssfwp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grjcxzgak.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gchrkjrje.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaddwbdkr.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/guuswhasg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gytqgdxym.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/ghabrqjyv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gxkfgcbfv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gopsnisrf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gstexbinb.sHtML


<!-- 参考信息 -->