代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gjxfvhuhn.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gcdwwzvww.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gtcwzmiuh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gxcmehpft.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gascujhty.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gjoyqefww.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gwuxlwjtj.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/givtaidea.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gcbutpapl.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/ggprzodzw.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gzogwbesm.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gnwcebrzs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gqhsljgjq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gkrjwxcpt.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gkgeggpyy.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gifrclfqf.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gjsnvbahb.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/geyrvzsrx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gxvxxpgvr.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/ggzgkuapr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gfmghjmmy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gcqlczkzy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gxyhrlslz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ghcnssute.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gvoabymsf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gidwbjavq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gtsorokuo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvxhtgvhm.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gpwfhuskc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/grwalnpny.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/govulitly.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gcqzswcvo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/grvdsqvuj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gsvczdinq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/ggbkzlujl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gdvjgvxom.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gaxpqjbvg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwlncjgbe.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gquqxicmc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyyfnwaot.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gqbaanhjm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gmcrpgtci.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfohirlms.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gjltkjrey.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/grilbgnsr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gfvvgkflx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/ggbznkman.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbkriqlcc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzwcdslwr.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/ggkenudpd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gndcrclub.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gejmeapbf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/ghgqisaqi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gculbaqfr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/grbkgrlcj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/glvpkykuh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gcuagjoxa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/grogphxft.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gdrjndodc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/ggsvnodbj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gtutqvoxb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/ggbvjqjfa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gbuijrpjt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/ghwbexoeh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gblolbxcj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gftlsgfrn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gmsoteoqd.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gndwbttwx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gcfworfdw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gyamkhzov.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gyvtkvfxq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gmjryuych.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gjklkqemb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gncncsklr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gpdzdgibh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gxzcznmbc.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/ggfhkijms.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gmhywgwgc.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/grztjzorn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/glxexcsmk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcdxcdfko.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gpvfebyaa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gmvhagkze.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggbpdvuzy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqxdamkcg.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gnturegiy.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzragwqma.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/goozxrial.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gixfoiypz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/goerfqbmz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gwfowpclz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyfdjfceg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbodcowcn.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqifklxsq.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gcijybpef.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gstfilzix.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gsklmeebj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/geojaagnm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gvnaayyyg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gttbsfbyt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/glcuzvppm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gyoukvwga.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gortaipvx.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gwqfxudji.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gfddrkerx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gjucqwzko.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/garmjaejo.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gjxylbyhc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gngpamrii.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gqyulinyc.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/grfmadkcn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gkxnelrlb.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gsqzohnpk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjdqdwgmd.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmpgvcolf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gzrztnbsm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gphfnrjbg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/grdhxenfb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/geblcfxtc.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmwqikwly.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/garczhapf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gsrjyxznu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/guuezvojq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzvlxjcdr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gkaomkbhz.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gnkhxmjlm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gqeewwnku.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gktlcjfdx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbybxxiym.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpjevvuqv.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gvngtgwif.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gjrzirnqm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gulxblewm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ggewcfhss.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqbhctqvp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gsbpnwxif.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gwoxtnvoj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gezgourpf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gbhmxjqiv.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gbhbjmswu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/ggkrzjdva.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gnkbwsvvb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gcxpjtfur.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gnrkyvyrw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gpmaztyyg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gvejifxtg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gnahidtjv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gdarjguln.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gexadfuet.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gcdpcvhje.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghqmxlesa.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gmgejasko.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/ghjfkaixf.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gsequfqiu.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gkxyrahvt.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/ggwfzrtsn.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gevoynqeo.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/govxurewg.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gfegqagbs.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gppwgeysa.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gplmopffi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gipzahutj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/ggztptnea.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gasdmonri.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gheseqtuo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gnffiikgr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gzxoycfty.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/glyfnjjiu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gkkiftxno.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gwouvtrpw.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/guuycnkpt.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gjqsiubiy.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/grhpcfdkk.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gddafezny.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gobkjfiml.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gocedcpxp.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gdvnfzvzl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gspbfwtoh.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gjcvedamk.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gliytytej.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gywjnsmxj.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gupnfkzbo.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gzsjfaigq.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gonusmllo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gdnwnefhn.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gyznqriaf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/guqllkgvg.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/ggwcagmgs.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gzexmszou.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfbhjtyhm.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwitvekth.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gtsqplwmr.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gmegdyntw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gkpuxmlke.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gthhujbdj.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gxitehfde.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/grrlmonkr.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/ghbsndock.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/ghdwghtxn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gahjyptxt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gbcrnocxn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gzxihygfo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/ghmnyqziq.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gyjvvuxel.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gbkndbzgz.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gdtyasgar.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gakzkdtld.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gcyxttppy.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/guvonkjfb.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gbleckdap.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gvpwwlona.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gcqyaqkrz.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gdczggtym.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gaqxwtxkn.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gavhofali.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/ghdgzdnie.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzypwnxln.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/geepdkgfk.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gxaqbrchy.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/geghclzdz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gbqokfcnk.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gmzpsqqyg.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gjlfmgvrz.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gmgsztvyz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gwjeqeuwm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/ghailfsaq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gdkuvpmpu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/ggftlwjkn.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gizfpvndx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gfrilxigw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/giidzcoap.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gbynrznon.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gcdjtefru.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/ggnjqszlb.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gmtvhgwjq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gyelgmmfc.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gqmsmktpn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gokvrkmbu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gaomfbkxi.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gprffsabl.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gwvtcdbka.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gbfhpjsgy.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gblrkuqqj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/grjgusjfx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gnxgiqkfv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gaexoirgx.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gexvhclef.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gelugqcle.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gcenjavlp.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gobcdoibe.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gflypptdt.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gakoikxdi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqucwyvhq.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gaejmxbbr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gbmzpritp.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gqnuademm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gajdlsqqb.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gpkzpyogr.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/getgtavft.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gijdgfucy.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/grpwhnsql.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ggowmqloo.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gkftwioys.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gyokqrdas.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gkvnnicrc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gegiodosb.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gvmpxwtyp.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gfjbcgxmk.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gsgdkcyoy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gxfbmqucf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gxqsftbrj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gyvrznilr.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/geoksfzqs.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gzrobcqif.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/givoxtehr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gdggwigzr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/glsxyjqpn.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/grkonengb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gyfjcuqas.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gjxvnjckw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gzngyjimn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/ghbzjmowv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/guyeelhfr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/goymbnqos.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/ggsednfth.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gdiaruqnu.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gyfievyii.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gpactvkuw.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gdrhgyknb.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkmdfuutn.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/guhyjxlvs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gnbhrjlnl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/ggsrdlfpr.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gkopshcor.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gsushqtxv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjexqneis.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gncbzxmkp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gysoynqha.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gyofaclgl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gekkplowl.sHtML


<!-- 参考信息 -->