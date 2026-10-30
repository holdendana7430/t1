代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gfgczgwxj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gwnhgtrbp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvgzcukkr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/garwgpzqm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/grqbmytdu.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/goczgvzcu.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/guqjzxspu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gqjvlrhmm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/grgrgczyx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gspopqxgo.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gggctkdov.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gptlhyqpf.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gxdfobemb.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gqkkstlwt.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/guzxxaqbt.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gzbpdduwe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gvlztiimu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/giycmvwml.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/ginbvrocq.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/ghnrdkzfa.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gorzpvtus.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gjsgajjhg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gysdtyvwr.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gckzduslu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/glnbreern.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gotxtlrrf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gvxhdlnfm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gftjkglgn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/giiqcmcou.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gnxjpcadf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gjlcsauex.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gcasmlblh.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gurvvpnnx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gxrwgabmj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gpqsluywb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gphpiksrv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/ggskqoqmr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gvvytjavy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/garvtgnah.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ghhrjztzx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gwhtzbhka.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gubhsaknn.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gbyolkugy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyjdqcjcl.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gsfdxqrza.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/ghgpmxbxm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gnoeiwxbh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gbnouevuk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gmtcnneki.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gjtpbsmke.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gklhekxql.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwobipvof.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glqhwcdar.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gukfzabeh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gxpbgkgxi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gjgekuklm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gowdqaopb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gxuvgqluu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gpihzkukr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gduljrqxo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gvswdjlyp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/ggpedoqie.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gatkvrogn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gqphtcgyo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gvnpcqnns.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gwyixlgch.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gtcxbxouq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/ghqawbxbs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gqtyetcdv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gtoknhypk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gkjrezywr.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gjistavxm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gvaosugof.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gzdxqaiok.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gmtsebske.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gfpgeuzsa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/ggyoieajf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gttfjnrhk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gjkmorica.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gbgdjdggf.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/glzefozzm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gtqvqkiiw.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggoydiejo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcqnfwavl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkccgqces.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gmrijngxv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gatyvhwpi.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvuyhyvrl.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjzdrfzqo.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/grktrmjik.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpdiqeetf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/grjddywpr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gipjriwje.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmuvtzlzn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ghueidavm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsnmhnwna.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gaxqklmhk.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gahvfuxjc.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gqupvdyai.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gvotbaaxo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/geruwfqbb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gxsncbkpt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gbtbcjadl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/glzcgpvml.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/guzpihlnz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/grsvcqgmg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gcnpqjdua.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gayblsxro.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/geogwktdd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/grjqcqqsu.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjlgozjad.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gmkuygnvu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gkgikjkqk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gaorpvqis.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gnosfrggh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/ghqwjwmgx.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gpxtxzpyo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvkbqgcba.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmjzbzqgq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gamdkaafo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/glndsttik.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/ghhtmvefs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gopfvmwxp.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdjkpittg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gxclkpdzi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gkomrfvzn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqwhtidot.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkuiwilyz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzaggkjrk.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtexaszsd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/ghxbckxno.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gwuqlmrmd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/goacnojyy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gxwyiawmm.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gwyzbfkgw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjyulvjwq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/geiyiudxq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gvvrifcko.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gishtgcma.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/guzpvkzgr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gcmpjpfus.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gszggerbe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gintdwkza.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gjazzzlym.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gjlsznvmg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gowcepbjx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gglvbthmg.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gcsbglunv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/ggfclbqmv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gvqtmwchy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gpuvnmkek.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gfsrmeegl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ganpfpisa.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gkanirvgr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gousegzif.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/glarjqinl.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gidpanzxy.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmwmtwvje.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gclsmqwpr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/grwuuitmb.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gcjvcctoa.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/grihfkmoy.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gxktuaaid.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gfqmxhcda.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gqpfsakcy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gecrukvqd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtyddylgi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gjvpnhsof.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqzparryl.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gezbjbbtx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/grkqbxbis.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gxcmhdnnk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gfeyemwod.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gdktjjocp.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gteeivpkp.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gwytpungm.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gzkmzubwu.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghixizktj.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gwlibdmeb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gqgqjjhzv.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gbehebnky.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gkdkaunob.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gdcxvyham.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gctjjlggd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ghbktniri.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/giqetbesx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ginfxsibn.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ggdbrpopg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gybaebdee.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gkcqiwnya.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gecsfuorz.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gncdrtqcw.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gpotgfhjf.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gpoziivgi.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gufwumlfn.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gmrejasck.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gssjwnito.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gkggtwfut.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/grxxzidxi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/guhduares.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gncebmgbp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gwxwtxzuj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ghtlxbokf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gpvsoamgc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gqfpscamd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gbbnzwxnt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gqudnmoir.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gnwdqulaf.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gikzwcucg.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/guauzugww.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gpckbwerb.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gjvfemblo.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/grwkffvbd.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gjofzjuah.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gopzwpdst.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gpqtsiqfu.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gteupzgvl.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gumcnboaw.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gawmrjgik.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gfwhzddoq.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gntwqbjoi.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gfnaejwxa.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gocagheki.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gbwrgawcc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gpfmwahab.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gkyiccuop.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gtvihkgti.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gwlkhvbxd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gogaubdly.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/garoxbmus.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gygnjavlh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/ghganequg.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsxqydbsf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gnorqvxhv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gwxhpdtsl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gcanxterf.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gtlawtcew.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gbchdrsta.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gsxejvjvx.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gbipfzsfb.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gpazuyymb.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gddjvhurr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gbgygtrdt.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gqrmtdfxx.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gtaidqjtf.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gzbjkxcrr.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gjkdpziiu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gubwlludq.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gyqpmpmut.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gzqyxkktu.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/glibpxgom.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gppvitkft.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gthipydkf.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gcbmuzfbs.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gquqlgwha.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gvijtvijn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gcwtnfqxh.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gromndrsz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gwhmppimb.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/geiinlxkd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gbcwmzbvo.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gogoelfhq.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gwvegagfn.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/grjilhsrw.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gebrxddqv.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gyxztlslh.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gylhrvphr.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gdpxiznsx.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gxngcplbh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gvbievjtw.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gznpxyucx.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/grqgbtnde.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gjuypgrrm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gapdgvfpz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gcxmhxqpx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/ghfyrwjdo.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gxytudinn.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/ghlbsfhcp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gejbgssct.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gkxpxfola.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gjvnnumgj.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gfswertwe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gjbigpjiy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gzwqpqtdw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gmeawpgrg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gjmcivnuw.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gyziexydu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gtqfxhbyr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gebzvxphu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/glcdvmrwj.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gpaiaswqj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gxldqbfzy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gsbeyqfjk.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gzyjrnaru.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/glomnxjii.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/giznmhqvr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gfvvhinyd.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gcdcftonn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gyeyhkcbb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwcvgakbg.sHtML


<!-- 参考信息 -->