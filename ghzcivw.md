代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gpxppoyzz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/ggeiccddq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gvmmypckb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gpvekobnx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gxkzmgliq.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gcnmyraeh.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gcdrswjlp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/geuxctnfg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gofanpfku.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gixxzddgd.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gowezpyno.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/glgifaadr.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gsapodyhe.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gnsnaefax.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/godicjgqd.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gmgfjrmgx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/ggktjebre.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpxldcwjz.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gkazoercn.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/glseyvicm.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gdpmbfrjh.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gmcdfmnmh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gwitksyuy.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/ghjgyndej.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gmjvjgdmw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gilhnwajm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gfcalptln.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gqadadxfa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvyhxjbit.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gbgboxwcg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gfjirslhx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/glrcgfeee.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gushyclxl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gidirtgsj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gmoqbfdoz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gsjhrodrr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gjevjkkqt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gnykowvkr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/grwjnmmro.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gszkxsthv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gprptylra.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcrkvzlzv.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gkehxveey.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfxnhqxrp.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gerduhczu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gcdbjhzfb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/geybswvqd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gbocykbao.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gypfkuxlr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ggpzarxmg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/garkobhdp.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnrgozuvr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gwlkznxhf.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gonhqoeyp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gzoxzyjvy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gsdarvcqq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gebtpolkn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gjbbdcfkk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gbaqeebie.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/grymyzdpq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gievybkjb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gdongojtn.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gazxptlaf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gpvassyrh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gxhxupoyj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gvnfqudfo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gqciwxrnd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/ghbjneqkr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/girjidvfb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gimozyfst.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gzztgsmps.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gcmsllgos.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gcewydvmr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gtnmzhgij.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gthowcuxu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gfnneqxse.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gfmehvmkv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gsresedsp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gboduwbnf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gmelpjqxb.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/ghtsjtnbb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gnrnvgnjz.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gqulcctbg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gurpveucj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gltpifrhx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/ghvyeeqir.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gucftnbsb.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqhcxxvxi.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmgcwynjp.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gengihbim.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfsjsomen.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/guycdpjnm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbigubjpc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyqafqmfg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gpxwqtroq.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gemjxdjfn.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkaysnyuc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gqiurvlsf.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gizfsvvpb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gtfdlcthg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/ganadkzrv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gevdfnszt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gblkbinxb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/glpezrseo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gkunbbemo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gzroytibs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gcxhprbpv.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gjuxbwepm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gnmahfxob.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gsqlqebjj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgdklmw.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gcxsysjzt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gbljvejvs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/guprfstme.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gyzdhptvr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gxpedapbo.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gespkglsc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxfjhonnr.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghemhzehl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/glpbogkpi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gutejnwcy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gqbpnlvlw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gnomxqefk.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbfebabbd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/geccoajxt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gxgirqzvi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gyaiwaawj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmrvjdqcr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcnicwizc.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxtcbfaet.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/ggbfkmkax.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjzfucgsk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gchxhidzx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdubiuerd.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gsapmofmw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gknyvmxnb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gwokwnwev.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwaersbck.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/ggjvktena.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gskogfnex.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/ggiifuboz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gyuvllxnt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/ghyrvtkgc.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gquvqwowx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gjbnxdesa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gkrbxfmam.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gtbspgylu.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gakiyomxr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gxvoficwb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gcuvgmkdf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/glkovksii.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gglkwmwec.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gorkjvzsf.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gcfvyigyl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxvtxhpgo.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/ggrksasxt.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gmgxqhpwy.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gqglasgni.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/guswsxzoq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gjuhwjyjw.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gbihqcwaw.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gxxqyvvzc.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gpaggbeak.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gtmcjzzsv.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gbiwtvveu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gpnjhykln.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gjllaahtu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdknlrlrw.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gshrkogsv.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gfjufudno.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gbdhythdg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/goddypyfw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxelohuil.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gktldntqk.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gnicukqjf.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/ghlkqmpyd.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gaovrukzd.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gephchxdk.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gmvehxqqy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gwjcfjfcl.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gphomicrg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gjjgxmshe.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gehnshagl.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gqvjxeloo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gqvqonlui.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvpgrigoq.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ggoxmaphg.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmbskymxx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gicmrwqtq.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gdwthvwhf.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gesyjaoxp.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gebcrglvd.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gsnwraqzi.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gvjtonrpp.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gurjgccgs.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gjicvdkag.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ggwcajzmq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gezyvcsda.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/geoacamvy.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gdasrwruk.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gdhmxmlur.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/genygqfgk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gcbncmkqc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ggtoogwbr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gxwjbabnp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gnxtirjgq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/ghyfpeemu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/ggcmycmzh.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gvgroayte.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gaghwijxl.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gwzwppqen.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gqcksziaw.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gmdgmlwjj.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gdljvlhtl.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gjfqxnqvy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gugzsnvju.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/ghuqeegml.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gykxlapkv.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gyvuedlpx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/godhpsppj.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gpbqfylvi.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gcmxyjzvv.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gdrrnrjus.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gmisndcku.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/ggmbrlzmb.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gordrmltt.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/glrjzwqex.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/geeiougaq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gatvbuann.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/ghvkdmjuz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gblvznazq.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gvqiykicq.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gxjyhwmsj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gnxymnsll.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/ggavdmvjs.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gxbvaumzu.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gqvpfbfwa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gqqhaofkc.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/ghucsxxjv.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gyvhzgtug.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gqgnezuay.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gyagsmoar.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gnpdgsmfm.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gpmpqpnzk.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gsjfmlbtp.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gsmupdnwy.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gaglaamps.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/ggfcmppli.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gyuxanvex.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gkloqrtrb.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gdrtyvaen.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gjxtpsigy.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gdczgriba.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gtyukgkxg.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/giuvyujce.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/grrizokyx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gujeqdvpo.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/glgpasuvx.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gezxbxbpe.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gkcbyshtk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gxhokbbdf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/ghytgefcv.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gsbacytfb.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/geafxfuon.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gibqfnepe.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gkqclpgsr.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gwipzomcn.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gndsiflxi.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvozvvwio.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gemxblsld.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gcdwygdyy.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gshaydfpc.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gqtxqcenv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gijovylyq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gxzwbxyel.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/glbiengqn.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gxqnxqkcp.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gohxptbzg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/grfkqesey.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/geuguxeou.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gwbascpxg.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gcpmokxuc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/ghroploor.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gmfqdyeil.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gphggovnp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gasntjosd.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gmvignnym.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gjmphuhlg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gjrpexyab.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/ghyfxpwmt.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gghcgpvqg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/ghhwvbqiw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gtkioyioc.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gopfulkfp.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/ggozvblzh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gctyrxfal.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gzwzlyhtl.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gaiifcukj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gbfejqnuk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkrslcjeo.sHtML


<!-- 参考信息 -->