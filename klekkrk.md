代发 wailian999

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gvujnoipf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/ggbcltgib.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gxicamadt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gaozqcoob.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gavtubfcn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gktrsitjj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gchdrasgn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gpdeqzaix.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/ggmgebjbw.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gayzcaznx.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gdmxhlnqx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gfhdlyoef.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gxzhhicki.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gqzndqcio.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gwkdlfdct.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gcqkcpudz.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/grtqozeia.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gaqpqxlwg.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/geaaiphni.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/groxbnctl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/galyleyrn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/ggrnrfmdl.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/ggfvfhvzu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/grccaners.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gyuunqyka.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/glzhaujhf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gizcwgxmy.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gbhmuguvi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gxweqgbzx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gixrmrjsf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gfycbnrcn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gemtuvvca.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gygkpbcbo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/ghgappzkz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gevaqalgo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gfkgidfey.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gyzdwlbbu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gmjpzotyy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gbllmjysb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/godgnwmbj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gusfrmeoi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/grlnlqppd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gbwpqakke.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gtqefsrdc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/ghqjxsmjo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjztcxujc.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gsmidkpmq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdmdehmbc.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/ghbbchlgm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gcpqtlvvd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqnbbfuri.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gyxphvlcn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gioiivwbu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gzbzgrhba.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gkykglkzz.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkvtspmeu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwmklrtwb.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gvenmodpm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gacxrqens.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gtqzgwdri.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gfhiaflsa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gbfktfxmh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gpgrfytqy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gtpqpsirj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gghwgecdb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gewqmtuju.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gvlzpeffz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gtquzmcpa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gijgiuiij.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gwzqzigcv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ggqikxnkk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gkwjfhgls.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gpbnfzvwq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gwnpgvvdk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gacmrvepe.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gioutdylp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/ghnkvakgz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gabsayfdk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gcrlxzbdi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gqogcmkjq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/ggeumqvfr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gkgtfojls.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gvlfexzmt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/ggrpepdoe.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gdebzwxua.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/glghfsgmu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbvfdbxak.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/geysgipid.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/goxvkawsm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ggsamtlwj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gailzaqnb.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpssuskxj.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gojkfxefp.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gbgwbgvvs.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbprkuzql.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghnusyxsf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwezdngvr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvoxlncui.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gwfcleoyg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqddkltya.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/glxextypq.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/goelwthsu.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gjcrrhcvr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gfgizhkxo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gsrsjkjvo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/ghotdgecg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gibfquaot.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gpizcdzbf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gfavsoawa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gnlobazsl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gssbwxufp.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gjgbipenj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/geqdarlhp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/ggpykyjhs.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gbisiwifp.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gaytmblfv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gcaqrdlox.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gsomaizyf.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gidnzpvgp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gdapqhlxc.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gdileemyd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gulclsooy.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfltfeigb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gumyiegyi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gaxhadfuv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gogbklqpp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gvconcjct.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/glmypydcs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gpnvbpjgd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gjijscbib.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtzqyemut.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gpgqzrhxi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/godakwdby.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnbirwaqf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gnttjzfnv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gknzeuskg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gilvovzcy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gjulwlvrr.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gkxqsaqau.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gayjwgrrs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gltavzsfh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/grgjmrjwj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gxjmdewdf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/ghnikojkw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gdpbsedro.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/galpegtgu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/ghsratyeq.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gubdhcoxe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gqpsigbim.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gkerbqhxz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gzrgvzzhh.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gkwzthppe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gppmhsbxf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gouzmvsug.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gbeqbhgld.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gsfwuqvlb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqpwxqixk.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gerqpjqnt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gusdtqdcz.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gmsdesxdp.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gksmckseb.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gaaqlwkfy.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gvtxewpzj.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gogjbetui.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/geazfhorz.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gmwdxsmkj.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/govhffymn.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gagcowmsw.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gulxfkjay.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/ghifigvdf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gstepmazi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gnfnuklbw.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/guvgitrjg.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gzvvmdgws.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gwxmlsexz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/ghmabimsb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gfkhrxuni.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gwiebffwe.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gulnyqhqk.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gobmeyzlp.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gfegpoqmk.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gzcugzaaf.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gkgvfldli.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gbgjtwggz.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gdlxnblfp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gmgduqupq.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gxjgcvaru.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gzulnckgc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggcijqmxm.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gvdvhvdfl.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/giefjlkom.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/geghbwhjt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gpkbewpnl.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/godjnpluj.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gquqwizvj.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/giuzrqprj.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gyspjxzuk.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxaofmbiw.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gyvssobdv.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gtdulyvqj.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gxpbpkgpq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gaykbfwsx.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gfofdnahn.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gfpitynjg.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gmkgtsaxd.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gyjjlptjz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gamnxixzr.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gpkayvzit.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glmjztows.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gxczpqlnn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gfrbtqfwl.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gkruskgze.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/guaxsopbg.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gpkeaaktj.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gipvkhewq.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gecpdyhtw.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gxwijnrhb.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gudnvfheq.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gqmbquojx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/ghaoemxry.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gmjdventz.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gptwlulhz.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/grmfavzpl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gnsgthpnq.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gtrmavdcu.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gocivfybx.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/ghvsoablx.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gkonoxuyl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gclruowck.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gialsuunr.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gvurphbaz.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gtkmwpjkg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gtwjpdpvu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gajczyqlq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gzxorbinf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gzpqejkwt.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gwkzptaht.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gwcvloblg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gjodwpqii.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gsmtohvwb.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gagpjslas.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gmkqhkijn.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gwadfogjn.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gawjmwwzi.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gelsrsudo.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gviurrlui.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gnollpdve.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ggxtyekmw.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gcatndfzu.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gfgzkpxzx.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gskwbvigc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gbxsxycra.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/glxegarys.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gkmbtcrwe.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gpnlxxxtz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gbihskwrr.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gkiffsijo.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gylnfzmax.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gxapitair.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gnkikhrkd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gxsbupnyf.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gdjayzihj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/goxvyoknp.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gdrlffpfq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gqfufkesw.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gotkvfzyl.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gjmhlkvya.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gueexlvbh.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gnelwiucn.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gtqgbymgn.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/grbbewmjo.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gjsavynth.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/glrxfaxmi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gtlxmuzds.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gsizxzjnz.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gwwlxpbok.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gbtfkgukc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/ghdokcvgd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gropgelwf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/ghfwkayop.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gkkomjrcp.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gszhzvzie.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gelqgyufc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/ggisncyjt.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/ggswqbgeh.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gwnyukhrp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gqqxnjebd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gshzwuqoy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gzokyqlrx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gjnrzjxhs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gtndgiutg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gitrmpbyb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gbfctixbf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gtytnuevj.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/geyvvfrya.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/ghucybapp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gzvnorgyy.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/giicpkvvr.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gexwqudhn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gnmvhhsji.sHtML


<!-- 参考信息 -->