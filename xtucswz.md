代发 wailian999

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gjazhzxzd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gzpoptzij.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gsgnsroof.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gtixfczgz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/giqdbmiik.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gcxecxkmi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/glcibnadc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/girfqogkv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gifshiapg.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gyodsagnm.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/govnibjph.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gdrptvrrw.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gghpfjesn.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gcaolkqmw.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gclsxropo.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gdofkapsy.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gfbqvuecq.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gjapbhyqv.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gmaoszoni.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gvurovcmx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gdlxxqazh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gyagelrhf.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/ghbyqsqta.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gnfpjtspk.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gceqpohha.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/goesnoeee.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gkqhscpgk.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gsxinnqxm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gfvictfhc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gqbrzkbdc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpiymwrxo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gqftbjyab.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gyfthovsy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gjokryojs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/ggzluoqtg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtkytigwk.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gwjexrphc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gwuyvutvy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gmsayljya.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gafphxvmb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/ghhabruiq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gnxqwdlux.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gfkmrsohe.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/grfjzjvpz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gjxyyfzds.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwoqxfxpm.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gjletjzfl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxrionwmr.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gpurqcrgh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gujcrpcvw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gcdjjyenp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gdlamcyaq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gypdluqrc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gcmyzprmw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/grinejttp.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggnqrbeoe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqrarpenu.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gmqvnlmrt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gkhmnwdnr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gupvzafha.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gxwlydhgu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gpatpezdk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gbrrywyyl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gicowecst.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gvpiolrmt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gvkmwstui.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gjbfykoif.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gvatzbixx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gardoxzty.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/glnsbornv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gzpivzanr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gcdcyfzyp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtbkcffd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gzzeyhxep.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gzfikidtb.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gstsrqixk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/grpvyodzj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gglzvleht.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpivqmzjc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gauxpmymi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gvqltzrsi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gpernekwd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gqyxddlyp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gxlqadrql.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gxavzoasr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gwfnriatm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcnrhnqtz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/grbjxxnsb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gskavujth.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/ghhyrrehf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gruzpcroo.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbctvesyd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gslrdvmax.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gugdbpnmm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfytizgxx.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkkyywnqi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggtzfzbed.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtiiviqwc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gtfbkuvrs.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsteefide.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gifjtkgmj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gaichqirb.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gouvxlkwv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gffjvomei.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gemirbhqd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/grggvxreb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/ghvvklrrx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gvtzjenor.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gxjcnbyth.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gnswkjzjz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gdhuzxbwu.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gjcdkausl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gvgdknauy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/geeokpnfi.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gqutcqqgw.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gslndhjpq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/giqrfjfuc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gtfogrkee.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gurvjwcaf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gymbbwjjn.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gfegnhpcl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtovllfgb.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdttlowor.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gubonsoyq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gjyudrckq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/grsfrveve.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gabppgeey.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcdcuoisy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gzgofxwrt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gddwrpnpn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gcynzbizt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/guvwdwoyr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpscwebus.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gogntxfcg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gvkzmzlil.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gscwabhjm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkgfrditr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpsaxfura.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gndegfobx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqvicazpn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gbmeypuqc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gbxfyqded.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gxteyglex.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gubhwewdu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/ghkipdcad.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gtfdktpri.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/glydowgla.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gzorzmskf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/guqwkjarh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gojfzcmcc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gesshqgmw.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gieejceqi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gkfcekryb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gkbaoktts.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gvxsbiwdi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/grppghuvs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glfrppbis.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gudljyytu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geevqtsqq.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gdisqlnca.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gdkrsjzac.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gtskplztr.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/ghplvzagp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gapgytbto.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gwsruexqj.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gguqygcpn.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gniivydne.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gffxoxqxs.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gwulqzyhv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gbsrtypef.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gebpfqpvz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/ggjacxabf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gmzvjuixm.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/ggvdytcsa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/ghrewwntm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gcudrnbpx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gdmfkczzz.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gebtnfbwi.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gfwchplsq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/giuiifymy.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gafidsdqk.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gxyusgjua.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/glwqqnloq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gmyyphahi.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/giaxktenj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gzyswlbxz.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gvjudpaoz.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gofxjatbi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/glturkqrh.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/golefwstj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gnfvprnkq.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/ghhvtvefx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/glutfvbfz.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gdofidqfc.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gfsfwapwe.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gfxqjacnr.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/glvylvokk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gnvljyxur.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gymkwnamz.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gqpdyxpvy.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfnchcqjb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gamjjjfft.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gkughyqis.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gfcjcxhvd.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gfxjukteh.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gujrzywnj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gvddkepex.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/goanxxiba.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gyaskrbuw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvncvaayv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gaplbokgg.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gxfkemkby.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/ghtyodgky.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gpvzmufmc.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/goszfaofi.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gxsatsnyz.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gulvwitxy.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gkaieckzm.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gqumlmffb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gclxqript.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gpxkcqscn.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gaydkaozl.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gcxzjgtrj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gdegheodg.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gcifuksfu.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gbgiakvgj.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gjkildmff.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gehkisutk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gajmolewr.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gcqnxohoo.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/ggwkfchhb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gsbhrqvce.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gwrogsugt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gdfxowsis.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gogbkgonz.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/geaoeaiqb.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gzihbitco.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gpmbugagz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gbaybvhdj.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/ggzsxjcfk.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gxgvvyhue.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gflykvfky.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gfdzujtiq.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gaaairvxw.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gegmsmyln.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gljmcwwcl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gpadbdscx.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gumyvfnsb.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gbchbvknk.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gyrxnujln.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gjmevzvtg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gktanbygf.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtpmkfnlt.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gehykgjie.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gvyocszlz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/grojvwpjo.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gbhtexzmr.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gruifrfis.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqpdqcilo.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gggqcpfbg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gutjuwevr.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcrgnnbeu.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gsrubfqrz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gslpdewum.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghlibcikk.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gpywszohh.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gqsgtkbmt.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gexvclado.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/glciarmxd.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gjrnoipyd.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/grqltfbwo.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/goaosqcvr.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gonnsvcct.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gxijyewkh.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gmaksjgzb.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gqnchbisw.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gnmxkmybj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gxusopdny.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/guoxgvohj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/grmyyszuf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gwqxgrjse.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gruooijqc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gztvmkwac.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/glnzyvsea.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/ghgvgqxnf.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/glpyhmtev.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gvlzkcwal.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gguaqvpgb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/geythnyxn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/ghiuuykar.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gsgcahkjz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gejfgpeah.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gkodrmbxi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ggzbpwwin.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gmcjkbwpv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gdaxjgbim.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gekodzuyf.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwxncsbn.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/geutxywqt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/grltzoswo.sHtML


<!-- 参考信息 -->