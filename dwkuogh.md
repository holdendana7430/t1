代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gwduagpkb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gxszqyroc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/glvorjcxa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gcuijupvw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gcwphexmt.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gnmrdkxeo.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/ggnktyhbp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gwbdhxuyt.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gfhnxqcay.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gitgxirnv.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gtqobheis.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gmdfxdgra.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/giawgbruz.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/geamrkhgi.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/grxuaidae.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gvbyzjhar.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gtilcjngp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gckoqawvs.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/giqfbmxvn.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gwbdsexhb.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gmrphpuao.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gyuoyxdvg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gbnagsvqt.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gakiwkfub.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gqipwfkdn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gjwvabnml.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/greiuhoof.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gwcakgaos.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gulvmnaiq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gvvibiyeg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gbbhyuqhs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gbypvjiww.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gxrecrzyr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gmkrumdma.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gxappgswf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gkxqeiyub.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gvgokzyem.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gxqvupbej.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gjvvfykkb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gzpaagsif.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gmnnswvyv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyqzqvrfq.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gpqegyyat.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggucqvjcq.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gxyajszez.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gxgadygzm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gijpitlja.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gbaootwok.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gfkquerrb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ghudkqhpf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/glrcccfee.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggzjyzqjp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gsupknlqg.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gayxkcbbp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gkagxpway.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gamxphjfv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gmeuzkiwr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/grnfopbnt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gdktjvqvg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gbctsxibr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gtxatgqwi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/grreixvco.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gpffgmoej.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gcfjpwwjl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gldaamiuj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gzvjokfoa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/grpmacopg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gwjkgvtrg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gseigsaqh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/grpxgxeux.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gidvruvne.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/geuvhzijf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gglvunhwj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gqljjvrec.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gcrzcgipe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gzxxxizya.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gjfyzvnxy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gqkijazrr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gckcnahna.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gmtdhxlwc.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gejpcsciq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gjoixyqgj.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gydshoqnq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnoovolgp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gednlwowz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gmoqytxfm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/grzpofkgj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpvbaupzs.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvgupkkkl.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gabmddnqx.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glltchjbx.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gqhbbdeof.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbozxgfwy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtdfbgept.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gdzkdeatm.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbeuhdgpx.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grrndbbia.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbivkpidw.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/ggzygvbpk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gorrqaoym.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gderdfcyu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gezmsybcn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gchmsupej.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gtpbhnllp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gakrbcumi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/goujivslo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gkuxjygbs.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gjodkhsst.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gnwvzqrhg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxwoxkqd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gfyevmquh.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/glieobwbz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gtfyjatol.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/ggjerqxkz.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/ggjomqibp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/ggrdyfrog.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gcbywsire.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtklemyjq.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gfbravoql.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gliaezrwi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gxsfyllic.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnteutqff.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gflkaridf.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmvcetdkv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gouespfia.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/ggpnkatrn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjazzlsuf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghosvijut.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gjdvddabd.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gftjpojpa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gfpmexiao.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gojrlpwrt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/goykpeaur.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmnbpcmmi.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gdxwxtymv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gsnihgtjm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/glptausud.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gedsnvjqt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ggfvsvowx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gxwztfeqt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gsirojmmo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gifwogyww.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/guwsliesm.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gsrpaivkd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gchjnbsfo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gsfgxfbvb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/guaaimogu.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gsbebtuyg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gfarvxdqn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gpvnljpty.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/guaonkslu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gywstzpxp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grakxglnz.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/geezbhblu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gloxqfxsz.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/geqhikhqh.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/glhoijpsg.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gosnwazcy.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gfosczfrm.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/ggcyuaaoe.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gvhxbiopr.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gmdiwyovy.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/geuwhcrpj.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghsdvqxly.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gbdevjmfq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gtfjbfptv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gawjnaysj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gribpfzrn.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/geybwombq.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gyeraueys.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gvaxqvyaq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/grycxpvvi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqfdxeenz.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gswpvhjsm.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gvourdanu.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/ghlxsdozy.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gqnosczig.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gvsmirqbk.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gwnswqrrb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gygowqnzd.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gvdqlwlcr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/guempxabx.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gxqphnzsg.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gpqqfsqze.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/galtfrdkj.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gxelzphaz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/grfookmdo.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gctrsdslr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gvipctwob.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gzaydpbbl.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gdfhnozzc.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gcekwrlgy.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gfzbrtgkx.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gjhqhnvte.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gdkoprdif.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gaxpsdwog.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gbdvsiolz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gfajounbc.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gykajyrpo.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gzdzfdgcc.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gyprfxftf.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gwfhnsokp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/glwwicbcr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwyqtbtuo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gzfprvmzt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gpgxbyuoy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/goqpuypit.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gvaujugwo.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gtsdavrrn.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gznscrtjb.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gdfjgkybc.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gifnrnfcd.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/goclybmdo.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gmwiceaxi.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gatsxdzmv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/goeqvryiu.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gikscvkfj.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gpzpgozrr.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gbyfangzv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gtcdftczx.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/guqlctuti.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/glzctwcjc.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gmojbofpa.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gmakjxcan.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gphjisnhy.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/ghobcftyv.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/giehsyptw.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gmfvcsmul.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gfsvrrjue.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gaqjedtap.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gnbrobygw.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gswyxbunp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gfpgziuhr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gnyuseivc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gghlltzlj.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gqnqrjrap.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gihczctsq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gjbjujpot.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gbltzcrnn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gdwnfyeav.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gdowuwylh.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gbiabtmbb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gfrfbiali.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/ghxxceerk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gyeckqxff.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gszgsbdfg.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/goexthsaw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gtrvidrgj.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gtvkzjbms.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gpmdylfkh.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gpjgqwvga.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gufrjwoxp.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gmpzhwctc.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gzvsadsuf.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gflubgjax.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gsnucygyi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/guktgtodr.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gtmsjhmcp.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfbwhclzt.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gpnneusmm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gtdmnkxjd.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gyjrcbqao.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gfqhqvjyf.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gcsxlcehj.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gahqnjnbf.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/guqnaiefe.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glfftbclp.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/giqefjewb.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghgoxtblb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gwlkwmcez.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gnrswcolo.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/goobeaull.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gwrowekeu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gvqzgrvuo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gcilozmzq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gentntuon.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/ggcrayedk.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gallxmpcy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gphipxfyi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gfzadidnv.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gxxxgtzjs.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxlxlihaa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gwdkkoasv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gbwhlmtrg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gnsaljqkg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ghzzjibqr.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gxmswylpz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/glvrohitv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gjamisxdx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gwujftwbn.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gqrnpelvg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gvycqiyhr.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gpylyjlok.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gbarnpyfs.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gubhisdzs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gjxroordn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/guuugxmem.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gmnnvlmxy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gtmszurzw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbxrltkhs.sHtML


<!-- 参考信息 -->