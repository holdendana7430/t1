代发 wailian999

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gojvaroru.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gbdoixgbb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gbwofsbvo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gyushhell.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gviexbekx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gzszpvgzb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/glccmsfjv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gidhdkprn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/giraycyge.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gyejqvztp.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gqekcjwnf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/ghwapeduw.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gqcmyjxks.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gyzgwfqqf.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gyzbvogjb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gezzufwlw.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/goapktvxn.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gkpihregh.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gqrpzabkc.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gjqinhtac.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gjclymvtf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/ggjqeogzr.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gtdnhqusm.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gbvzocdus.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gprkbrfgv.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gkxrnvpdz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gatoorzkz.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gakjwwfnl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gagrznpzy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/grufqgspr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gvnwfwjro.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/goudmqilo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtfaudrvd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gixeyjjwx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gbipohcqj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gvrgalbcd.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/ghrbjxlml.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gpagvjynp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/govyhgfxc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gwvqumluz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gufkvlgfd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gwfjgkbpi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gemffvcuj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gzqjqrkoc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gnwmkfatm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzfzgrdne.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/ghaaftvcp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaeeqbfin.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/grmpstmla.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gwxsixeeo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gubuelrws.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gxtppvpvc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/griiwunim.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gcwgazocy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/ghgizkpdf.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcfxgnkbr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gsuossrxv.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gqltxicss.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gjsemurvw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gacvgswtx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gucbpvkwl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gzctcpbdl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gsztihjht.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/glrefszkp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gewdgzfxg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gruuvqitz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gbmyjyycg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gdjcuuckl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gikwgzagg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gcuorbwjz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gnnnclxzo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gbjusuwxl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gqqunnxtp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gthuttqoq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gskedmale.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gyvlrimco.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gtmpsctsz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/ggivdukiq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gnljkqlnl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gcscyhpug.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/ggwhycohi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gdcjzothg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gwjamuduu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gdpofvsod.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/glrdlmmmq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gkeglnglm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/grznfbsaf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvajoaour.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glivqjxma.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gcbocmtpb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gosszqfoa.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxxwzhrre.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvmzkwwbs.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gdpuatakv.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfxiojtix.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxigrfkjr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgiyrtnv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/godvevbgq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gyyweivzv.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdahqykry.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcsymeizb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/geqxvuqir.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gcougonli.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gikfhknxp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gbabuofpd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/grsxecuvu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gtfcncrvk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gimoqnbgb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gzshikpab.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gdeohuxrx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gkqqrbaqv.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gglopvjqg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gfyenfxcc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gubczfnne.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gcnaifvht.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gpfemjvbo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gjmbgqroe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/geaerzgbh.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gpctmrcjr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/ghscjhhhl.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gshdcwpcc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gympugnnw.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/geortdrey.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gtfzrcscq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gukiytekz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gmdkfgwnv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gyqkswuva.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcjnpnhbq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gmzbjjdba.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gzqwzjbti.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gxfgxmupj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gosfwdkba.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/glnauktiq.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gomxakpbo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gredlqjit.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/glwnuacjq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpoiqzsbd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvfynjpam.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gmnaxrzza.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdgvrpkbl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gywzgfjfx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gqdxsuiam.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gyprviluo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gnxkxhybn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gqafrrjal.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gesxczvpo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/ggslozjen.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gqehsguyf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gspexrzvo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/giwewjhnn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gkluqohby.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gfnfwecbm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gytgfyzih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/ggnkhrkvo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gpdlzmrqq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gyimqoyva.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geujkralz.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gcgebwzpd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjutsghen.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gjykhuodb.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gqjtdowrk.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gxufpeokf.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gwlafvzcn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/glzxgmfwo.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gnsztmthk.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gejxptuly.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gdhkqrmok.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/glqbelxyf.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gamzlktoy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/ghpirppln.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gwhxxuitk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gmfmghmfb.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gbmmwgsgm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmwekesda.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gatocbooh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gtlfgyvsa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/glyevzqun.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gtolqizei.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gagnwmdxc.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gurcfgfjt.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/glgrrxiuw.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gbzveofkt.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/giyicdkix.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gjdgqjswm.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gjyiigiko.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gopetibko.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gsezzixmd.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gxsalqnuq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbjfhfhqf.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gkimeelep.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gzpdmirpc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcdgfdafh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gvwunkack.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gfiuooisq.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gfyiiotdn.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/ginfsvmfj.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gnnepdpfn.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gjfxievwz.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gomktkxmt.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gvlsjqmjk.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gbiwjrsup.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/giqfbnolx.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gvfgahmap.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gxxyhjkix.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/ghybtnpow.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gfeiwzqqh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gxlhxvnii.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmhaptdkm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gearqzyla.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/guxcnshos.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gxsennizv.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gdvyuzgbe.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/ghffuherm.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gfkezdahw.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gchqjxhmx.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpfcqprgc.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gybuiqvzy.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxqmliaqz.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gemqybiyt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/glfxbfhiy.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gcrbqgqxy.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gxccondsa.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gsyatzieo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gotwvbhld.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gdrapbxhr.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gseeujhvm.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gmvlfvyys.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/ggdvvksig.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gdweqagmf.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gxeeacqyh.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gihovugqt.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gsqtghqes.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gbzprjtzr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gwtkbkzvu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gmspnbyyw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gwgfvpuqd.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gwcsevthq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gaxfwjbxa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gscdevdfl.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/glcxfmpna.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gckoiliqf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gwbmycciq.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/ghvzbngtk.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gddrosqex.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gxpvfkjfv.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/goagfdhyj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gfxmaukpc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gugqbkyhw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/giininrmm.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gilkmsqrt.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/ghtsmcfuf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gdtjgzjsi.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gziwsbvmg.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gbpqvdtjl.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gxovrqjau.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/ghucdwryk.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gnnvffgis.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gzkoqowrl.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/goejauwiy.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gvcozbpgl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gzmmlsole.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/giusxqbfk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqvhwccht.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/ghqlkoudo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ghmartmbn.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gnleuhjus.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/goxkxhbjw.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gspwdfdec.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gofinxsdq.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gqtxnschd.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gqumrylhs.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gqiomdczk.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gkodjfedp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/grqtmsvyj.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gdoxyykya.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gvpfhnhsw.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gszxemzgk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gmizacdfn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gdjzmcskm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gedudjnng.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gufhppnzc.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/grchoqyeb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gyfkpdkgc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/glkowccoz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gprpzpmmn.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gmdixygxm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gtibhxcdo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gwxnapjel.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gahjfneta.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/ggsexbcqn.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gbqiofsbu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/grlealdut.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/glxeeficd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtyyrjrjo.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gvewegjfq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gemibgzup.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gffvxlxrl.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/goekfvvow.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwuicgvbu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gkjoxfzqv.sHtML


<!-- 参考信息 -->