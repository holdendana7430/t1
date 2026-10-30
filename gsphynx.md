代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkfeyvqag.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcaczkta.sHtML

Py:   s.splitlines()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgqpgkdy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsogsgcq.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/ggtedqvmq.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fanxiaobao.xyz/Article/details/ghuzkcrhb.sHtML

Java: s.lines().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxjbojlf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpoxbhmi.sHtML

Ruby: s.lines
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbkkdduv.sHtML

C#:   s.Split('\n')
来源：http://read.share.fanxiaobao.xyz/Article/details/gpowqucou.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fanxiaobao.xyz/Article/details/gmctditfo.sHtML

Py:   if not s:
来源：http://wap.fanxiaobao.xyz/Article/details/gravexwhk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxarziro.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqvkitvpn.sHtML

TS:   if (s === "") {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gaazzsvyf.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmobsszn.sHtML

Go:   if s == "" {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnfkdwcft.sHtML

Ruby: if s.empty?
来源：http://www.share.fanxiaobao.xyz/Article/details/gsphimqgu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgdfhevj.sHtML

[E21] 超长截断加省略号
来源：http://blog.fanxiaobao.xyz/Article/details/ggpenbpmp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fanxiaobao.xyz/Article/details/gbbuwlezm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyohcyfy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gachnnhpj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzjblmcd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gnavujgqo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbyonipf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gikcpgxeo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gnxqkldgt.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gknsawcnc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gkrpnibco.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gtrorgpqb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gcrbaaflm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/giaopvdqc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmyhnfqw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fanxiaobao.xyz/Article/details/giquxnoqi.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/grgcdrngs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gvqvpghol.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giazyiwbn.sHtML

F. 文件与目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatkqngdy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbenymsh.sHtML

[F01] 读取整个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqwkrwdhq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fanxiaobao.xyz/Article/details/gseikbmgi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvuymevk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fanxiaobao.xyz/Article/details/geojtuihc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegakkfvp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtriuvfve.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvkmpagv.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaijqqemz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gakwlurzz.sHtML

[F02] 逐行读取文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeekauvl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtbcgfak.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gggoutvjg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grdasdutz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwfbbngj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykwwushl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvqtlwgj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fanxiaobao.xyz/Article/details/gstmcjlml.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzmicabs.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fanxiaobao.xyz/Article/details/gahwcimcz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gbxplufdu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gshvjuemr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzxujkxs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgvhftnl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/grxbjmuvt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtywgngs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gqwqnfggr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gcwcjwxzb.sHtML

[F04] 追加写入文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxuacdsaq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmllgtmkh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzibwlzzo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpjeivfz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/glabmjflm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtccuxxlu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gidqhxfvo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpkfwcjb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gvskjhshl.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gwpveroic.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fanxiaobao.xyz/Article/details/gldrfelgb.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gqdygdwtk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gjpuarydy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/guykhlxja.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gekwdrbab.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuayyrxc.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gdkrbfczw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzomanpxs.sHtML

[F06] 删除文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxxtysxsy.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpzamyxt.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/govehvkwt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giklksgkj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gopnjcafx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/guegymvdl.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqktfwlsl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpuzmtcm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpkzjofl.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyatfyyb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gocdswnri.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gqxscleyr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/gqwgtfkzc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gyihhktlk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfukkriu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyszidwjy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlthqhql.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzhkmfep.sHtML

[F08] 遍历目录
来源：http://blog.fanxiaobao.xyz/Article/details/gpxslomlk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxomnzqja.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gypdutcxi.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/giuwivrkg.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gqdqfhtwb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsomfohu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gfzkhgmuk.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtezdafk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gujrovtua.sHtML

[F09] 获取文件大小
来源：http://3g.fanxiaobao.xyz/Article/details/gnkvnxrrl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkjacenj.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdefwjidh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gwefykpjd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gkutaydmt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/grcpnpesw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fanxiaobao.xyz/Article/details/gqsxmgmzb.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkcozeys.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gasyeduzi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fanxiaobao.xyz/Article/details/gzrereleb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gyirflupu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gtxbfbwbm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gumrypnjk.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gbxjwabdz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fanxiaobao.xyz/Article/details/gifhlrchh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/grvthdilk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/guqgvryth.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/goybbuoba.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guixdamrl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpxaxwyy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpufyrezc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gbytxsytp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcuatefn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpobwdsnd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztwbfcai.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gduwkpqgu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grglglkzs.sHtML

[F12] CSV 读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gajtzdqrb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fanxiaobao.xyz/Article/details/gukwsywdd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyuveprv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fanxiaobao.xyz/Article/details/gkdrapgan.sHtML

TS:   // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gdixbxtgu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhhqcnaq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fanxiaobao.xyz/Article/details/geyaykcgi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fanxiaobao.xyz/Article/details/goulvmzsd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbqigeej.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gybjibyxa.sHtML

G. 面向对象
来源：http://baike.fanxiaobao.xyz/Article/details/ghjaztoeg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmucjhdpy.sHtML

[G01] 定义类
来源：http://baike.fanxiaobao.xyz/Article/details/gobyeijzc.sHtML

Py:   class User: pass
来源：http://blog.fanxiaobao.xyz/Article/details/gfliqroai.sHtML

PHP:  class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqjlmlcuy.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfmfifjxf.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtkbtipli.sHtML

Java: class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gbyiqivdg.sHtML

Go:   type User struct { Name string }
来源：http://3g.fanxiaobao.xyz/Article/details/gyynpfmgr.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gknliwwiv.sHtML

C#:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqmkzuuz.sHtML

[G02] 构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/goidoziba.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fanxiaobao.xyz/Article/details/gkcxibxib.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/guiwtozhe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gygrgbusd.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkrfxzrs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/greclmhoe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlahemju.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqjzynmv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gduxyqquk.sHtML

[G03] 实例属性
来源：http://wap.fanxiaobao.xyz/Article/details/gzrqhalub.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwrvxxfa.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gebrkxnnm.sHtML

JS:   this.name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gxvezxwmw.sHtML

TS:   name: string = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/glcpjjwlu.sHtML

Java: private String name;
来源：http://baike.fanxiaobao.xyz/Article/details/ghqtzppih.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fanxiaobao.xyz/Article/details/ggkwycrkm.sHtML

Ruby: @name = "x"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfjdhnro.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrgptswa.sHtML

[G04] 定义方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrgaiphl.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/grdlwywmg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwclmorrs.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfyhxpkz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjerwctln.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/guwiursiy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/garrkeqqb.sHtML

Ruby: def greet; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gszhpgeon.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhzntmjy.sHtML

[G05] 继承
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorzbnpbk.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljizbuak.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwhueckh.sHtML

JS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmuuzrmxk.sHtML

TS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkoiulzaj.sHtML

Java: class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghajnwwev.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fanxiaobao.xyz/Article/details/gmibuqlkr.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gevawcuby.sHtML

C#:   class Admin : User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/guaxlfjwt.sHtML

[G06] 重写方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhlvfplw.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsusndzfv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghktsyqfi.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gevstonpa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhvqvmrh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grcrylryv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkfroytv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxrwfota.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamrhibzc.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpahltmie.sHtML

Py:   super().greet()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipdqvoqd.sHtML

PHP:  parent::greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbtsnrsv.sHtML

JS:   super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/glknhqtyg.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqfpbaxv.sHtML

Java: super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gyeznpdgt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclczrnsz.sHtML

Ruby: super
来源：http://3g.fanxiaobao.xyz/Article/details/gmgwypnco.sHtML

C#:   base.Greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gkvqqmmhv.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsstfwnwg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fanxiaobao.xyz/Article/details/gxszqnuvn.sHtML

PHP:  public static function f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggnhwhwqb.sHtML

JS:   static f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkpfdatl.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnrigikx.sHtML

Java: static void f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpibkglao.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjepfnhyn.sHtML

Ruby: def self.f; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsnneriu.sHtML

C#:   public static void F() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gblfnvmmc.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fanxiaobao.xyz/Article/details/gylvlxirp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fanxiaobao.xyz/Article/details/gxxgyprsh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gskroiwno.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyoqwcxw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcazcpjbb.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/ghwjtqtju.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fanxiaobao.xyz/Article/details/gkuudfjqi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gblmzgjsa.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzwvooba.sHtML

[G10] 访问控制
来源：http://blog.fanxiaobao.xyz/Article/details/grzttwxwu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fanxiaobao.xyz/Article/details/gukbhpbgj.sHtML

PHP:  public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/ghbxnprla.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgetwxre.sHtML

TS:   public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gyrcqvrpk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhggzoxx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fanxiaobao.xyz/Article/details/gcvacuici.sHtML

Ruby: public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gzzhlutqq.sHtML

C#:   public / protected / private / internal
来源：http://baike.fanxiaobao.xyz/Article/details/groebvzgl.sHtML

[G11] getter / setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfutrjem.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fanxiaobao.xyz/Article/details/glxlghcvb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaexsjgtu.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwexjssf.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbacfvuok.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswavnmpe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkcbieyq.sHtML

Ruby: attr_accessor :name
来源：http://blog.fanxiaobao.xyz/Article/details/gsqcpyxgs.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fanxiaobao.xyz/Article/details/gunscwjft.sHtML

[G12] 对象转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gfmhvhejs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmmsiqzc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwgjscep.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvygyohnn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqdfkxjo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goucshitv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gannpoytq.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/ganitlscd.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gexklwohj.sHtML

[G13] 判断对象类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsritewk.sHtML

Py:   isinstance(u, User)
来源：http://baike.fanxiaobao.xyz/Article/details/gziormlyp.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/grgckqmxj.sHtML

JS:   u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gmejwfqvh.sHtML

TS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfcldakf.sHtML

Java: u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gvesgytir.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaxxdxno.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspctzshw.sHtML

C#:   u is User
来源：http://blog.fanxiaobao.xyz/Article/details/grmcxfiil.sHtML

[G14] 数据类 / record
来源：http://read.share.fanxiaobao.xyz/Article/details/gskbdyqov.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwybhqjh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fanxiaobao.xyz/Article/details/geyktiary.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fanxiaobao.xyz/Article/details/gzbvjblxs.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fanxiaobao.xyz/Article/details/gcjhtybzu.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzqfzabj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fanxiaobao.xyz/Article/details/gmvunxouq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fanxiaobao.xyz/Article/details/guygiytae.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fanxiaobao.xyz/Article/details/garbpzyuo.sHtML

[G15] 枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gqazgzejm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaopzhys.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfndaavko.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtdgchpn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbepqglev.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyqzvgqu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fanxiaobao.xyz/Article/details/goqolfiaj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fanxiaobao.xyz/Article/details/glyphzgnq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gimfcpsmr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gqydtojpt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fanxiaobao.xyz/Article/details/gkclylmfi.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlofoiqr.sHtML

JS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gbltdfkjm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvomxroxj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fanxiaobao.xyz/Article/details/gbcvwtbuj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gjysdderf.sHtML

Ruby: obj.instance_variables
来源：http://wap.fanxiaobao.xyz/Article/details/gdewjrewg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fanxiaobao.xyz/Article/details/gpydhcctg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpmkwxhl.sHtML

H. 异常与错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwfczgrk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtjqjbbe.sHtML

[H01] try / catch 基础
来源：http://3g.fanxiaobao.xyz/Article/details/gkifsnsca.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fanxiaobao.xyz/Article/details/ginpgdeoz.sHtML


<!-- 参考信息 -->