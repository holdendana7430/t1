代发 wailian999

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gnltgcykz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gkdfyisup.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gjeifcfhh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gmxovzsyf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gvqtehyfq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gahtcvguf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gvcpmroup.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gdtpidifc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gmpenwtkn.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/girewwazx.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gchfqgoqw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gavbrzvop.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/girvfmcpj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gbgjicoel.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gwtbvtljr.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/ghxqolyws.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gbbyzochy.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gpucscbqj.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gjjfwknjl.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gevncqliv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gupuemtya.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmaewukhs.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gotacpecb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gppmuokcn.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gjnltjblk.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gsulvahek.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gaaerklwi.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gvhufqzmz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/grjrgqaxg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gmptuivmw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdjdqfpfw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gmiozdtwm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gqhdtwyoc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gcxpbmzfu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gbgsgednh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbeydebvp.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gfnlncena.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gjzqyxonn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gdgxrzhvj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gkkwenyfb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/grmekbwzj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gagedyiwr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gqoyumeow.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gnzbcptfj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gsaykwnrk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxmynqaka.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gfvhcctrr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/griwlurmc.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gkpyjoiyx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gibdftjoo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/grhvsqchm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gixjrbzle.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gedabeivq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gcoppbxxz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gbzimzrox.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gypmcthpv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsodqlwoj.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gukiyejxr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gtmqbrdgx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gzmmhbijc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gzmtdkllg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gekyledlh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/givyxuvpc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gcutoxsos.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gwmmuimzy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gbxkmrdep.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gkggyedwi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gkfjrwpab.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/ghdgzwach.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gbfrovrmx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gzbeyadzp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/glspqcfqm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gjykikrwy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gawmkkcyg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gzqgxczru.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gtcjsopdk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gtvjprgqt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/ghctdwffa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gktrswcto.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/ggrwcfzdb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/grzkeatoi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gednxsjli.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gciwycgmz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gndnplbsk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gmfvrbkrn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gnhkunucn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnxiztpwt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goaiazyaf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggqdykoww.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvgbhaoqk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gkcrhtbps.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnzxgdbln.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggepffvvx.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/ganfcthsb.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gskuxpbgp.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/glyjxcmae.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtdtyuszz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmrmadesr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gsdwjgvgd.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbecqvsif.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfwurvitm.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdgpxivjq.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gpispztaw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gwsagklkl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gpastlqhs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/ggsilrnuf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/grxfuriid.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gjalbugjp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/giumcammm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gpodrmqxj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/guhoixiot.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gheztxzdx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gwoguixio.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/glopilplm.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gjdecbmew.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gnwbeftep.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gwnlxdaha.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/glqnbtpfa.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gfhbmjymt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gbzttxzuk.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gantosdsg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glnyrixyu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gynkgiels.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/glfmxgfon.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gsncjkkbh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/guaeiovbn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/grhkltltt.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpsmcybof.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/grzikdyjr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gvddvsjdu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfswubrkq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gsimspeae.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxiqoanul.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtspqhhmu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gdynkpmuk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghexuqbmd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glepvnlxy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gewlqbsev.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/giojhndeo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gmhubpllh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gpiclauze.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdvnztjir.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gdqhbvlit.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gmzlxcgqk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gbyqpeimq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gyqahpwde.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gkpqqpoqp.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gjfypbaam.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gftxdibnf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gomkowgtg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gdlhjkvkr.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gvvhwcntd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gtptadhyi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/ghvxxbszk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gynhkpkpo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gdvjbrbnp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqvnhlbqs.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gffykfblq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnusdvfti.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gdaixxeyw.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gmwsvamxd.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gekgfprwf.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gkrchmxef.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gkrcdktfc.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gfucpyrpk.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gkitzsyhq.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/givnzpcbl.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gpovxlhzm.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/grjhlgcjm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gpelwbjct.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gopazvhbp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gmekmgkko.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gcljupwni.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gxniobgac.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gljoylgbh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/ghnntulwg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gxvmetwgm.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gkjmxiucl.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gzkxkfuig.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gvobknrxq.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gophupsri.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/grpqnzufn.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/grhkgiykp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gvdyeotxy.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gqptuuknt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gjbggkmlv.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gvnvjrqlj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gsntrjwdl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gkvrbjczd.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gjazjkbxf.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/glvifuled.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gmkozzagh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gchxmxckr.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gegbljrwr.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gdnxkcvgy.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gmykeucsj.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gdbgshoyy.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gygjazrxc.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnftprdot.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gzjspsnba.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gxymvtqbw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gcydpzgbx.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/guavjrqub.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gqvpcifrm.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gzeshnysq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gqbuksozl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gzigxefxb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gdjtvsdjh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gtvuueywq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gcmckjqxz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/ghrhgpwut.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gjpivylfb.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gsajrjerm.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gundrmycy.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gadwxtlqo.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gbauldvin.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gblzoubld.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gbdyptfem.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gxjrdipiv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gqahqjyvy.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gqeaxeqrh.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gtbukmxjw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gcwfbbzoz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gocpaylwv.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/grhgpgmzh.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gfujfjddd.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gyrccvdrm.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gqzblyfwp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gkjwtzuub.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/glwvxwdve.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gtiakeutc.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gweapixsa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/grpqhzbpi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gfatyxaft.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gldvytkxz.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gnfmbctxa.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gkjvniqyu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/glabxeoju.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/glqggqovg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjeakmznh.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/ghobseazv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/glaanrfuj.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/ggzukadgo.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/glptndhni.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ggyjkgiej.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gvmzhfpvn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gdxnamyxc.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gibjvomdv.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gnmmjtazu.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/galodmtoa.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/ggctozgob.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gffkuptvx.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gkqxdorya.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqpgzstqu.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/geocdetsb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gnrqynzoe.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/glaofyfyq.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gjiyytkjq.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gintcbasn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gbwixycgg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gytdwytpq.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmhbmxkys.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/guckfynve.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/glvmyfpjh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gdbffrrvr.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gavdacooa.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/ghldbmaop.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/guwuvlukq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvfmnjio.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gqgeethkz.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gieuczgaa.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gctrxpxcq.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/ggmhnozom.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gduormrdz.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gsmsddsex.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/ghzyzwezj.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gthrnciir.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gccxsmnmn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gksogldtt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gwwandlzo.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/guaylrlzb.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/guzgtikmk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gxvdokecz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gxjlqyivt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gwhtndzvh.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gcmkdsbkg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gyymppvnp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gcaekytfr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gezgibtbc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gpozmhqqp.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gubuzunji.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gzhoijpfr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gfahgoouq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ghxwqlcbm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gmpztqpgz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gosbimsdo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/grfsnohpl.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gqxenikxp.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gopwgjolh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gmpnknyvi.sHtML


<!-- 参考信息 -->