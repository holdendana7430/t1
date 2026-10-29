代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gtenamacv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/giucxvchg.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gztxvvxtm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/grlwiklrp.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/grsodgnvi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gmscfjjlb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gzfyjvxuc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gfxljrubh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gawqgfbnv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gdyvdunwj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gpcyropkv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gsxzjrkvd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gquowteza.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gkmlifwio.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gycmzhfzm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gotkxkgda.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/guxucwqed.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gfckgdwcz.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gwlvljhlv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gzxnvgznd.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gtyvjgpff.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gqmosoxpq.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gavvpqspn.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gzueqyyng.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gfknirdnr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gubqkrzyd.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gpyseqfcw.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gdvhfjtcv.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gumaxiqfk.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/ggngmksfm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gzfonmgfz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gtcggdhik.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gtjuvpvtf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gpcgscrth.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gwbkxzmxb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gteuvckma.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gqqejajkp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gttpzkifl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gjmpivbin.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gkxikjrec.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gwzejkevf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gwbitzals.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gcazthciu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gtlmxdunz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/grqxwbibr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gmkpojppg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gqzdmveqx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gtzywcpbe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gttadwbrg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grdbpgsnn.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gvxfodacc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfmtgovrn.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gmvszicuf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gwowbktab.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtrixxind.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gbqqftxcn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gkrrwfmaa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gfbjdsrtv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gbumthcza.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmzxwwkat.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkbcgwfpo.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gqiejkpao.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gvpbwkqro.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gkdwzzjwq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcrmanoyv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/girqxyjzj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gvrxtweoe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gbqrvekbe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gtuftcoei.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gdiksmoue.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gyhcjwbic.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/grrilkyps.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gtnlsbnsr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gvwkzcwex.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gltepcuxe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gvnglceoq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gljojjfax.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gsafqmawf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gvxwixctf.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gevjbakut.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gauxqhwyb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gizibfwpc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gnkeyrpue.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gkptmnztm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gyhqosaxr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gjiokvrrr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gflvqusha.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gotumogbk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gaoiywpdy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/glzqdtnbc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbqkuyukq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdwsifgws.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxmxevrlz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gsrytyuef.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/grqynqbqg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggbsjxjxt.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdeflcylt.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gmtdctjnu.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gntwzedbo.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/ggpmtjxws.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbkrrdxpx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbxwuclub.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/ggoftvefc.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmrqzbnro.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grmzopowz.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gwfbtyxip.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gttvbaomr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gmuqmkjad.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/grxnufdnq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gxddqnhjj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gmidvqlbd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gvcnbajlz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/guupkatyt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gxloljosr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gzriluqte.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/goedmpijj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gjntpjysa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gyfyzshbn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjkyilfxw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/glgviasic.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/grjmbsztz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gybmscujf.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/giedkzqah.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gaaopydxz.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gzppvbasa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvxkupzto.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfvyyktxw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/glxccrojx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gxbgwmems.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gyiwsozlb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gsuqijlce.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkhehmevi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gqnxfncig.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gxeriskpz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/garkkuqlk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxeampjgh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/grjcgufad.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/glvduskml.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/goeqkvgys.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/glygzbvek.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzlnvaamo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/garngtddt.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gskwymocq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gklemjunh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gkvgmqpdi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/grcpwhksr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gryybxody.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gwbdpznoc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gclglscec.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gtxkqkwlr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gsplpisht.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gdsfvaequ.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gwxegcfpt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gyffbfcyn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gitepksfp.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gnvkiheof.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gemylpagg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gvljrbdfy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/grwmumafy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gozhqjfhg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ganaucznl.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/geetydjjd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gthzhsjdp.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gyktviobm.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gvpvurrpa.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gapkflokp.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/glfnziwmx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/ghpbpcbnu.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gitfddxsf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gojkakrvt.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gerzpedva.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gnxlaagsr.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/grqzxyxpg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gueyivjtz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gychdqbxs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gcsjpdlpy.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gtmhrswcm.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gafydlicb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gehvqdout.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/ghbvtwsdn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzfojaxz.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gmzbaehcc.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/ghxfjvzmo.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gplyvuogy.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gztktjgih.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gkbzevzjm.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gbluokuga.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gsusbpjnc.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gyaiiblcd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/grwbfydbc.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/girdmwljz.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gjgikesdy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpdvhtdga.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ghwosuwul.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gpgtnsmtn.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gjdfsolyt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/ghmeproll.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/ghkwzkhua.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gmwlgvrvi.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gwtuoccfo.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gepunlehi.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gfztourwo.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glfguncps.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/givxyedgg.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gaglrdvth.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gckglgses.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gdsyjjcys.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gojuqyatk.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gurllocod.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gsewmwmrp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gffikrnqc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gehaxezwc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gkqgcvota.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ggczlssgv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gaybnggoe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gueipgfzt.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gcxvuhwqt.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gwoqwzmox.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gjibaqdtc.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/ggjsbhbhv.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gyavdwlfy.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gbvgatutj.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gcosssmdg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/griitynoj.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gkwplaybm.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gliilawcc.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gbkukdyjn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gxihwquhp.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gutyrzxmj.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gfbkxuhei.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gojbowpgg.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/geqbgvxzl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gpxcuwwxt.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/ggefzdzgv.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gvatccoys.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gaokfqqea.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gtccyvbli.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gocheltta.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gulwvrysv.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/geoqkmrnp.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvejqrofz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/glchxvlxt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gcqyiqnjh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/ghxivbgko.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gnrjikmge.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gwdqszrnt.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ggbolpbdg.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/geliwaahy.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/ggoaafaka.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gjmvlqmqy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gdifilhhc.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gupawulsg.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gtzqusxhb.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gpuprmapq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/geqhwwuuq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gmxvyczio.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gmhxejggw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/ggmuilatb.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/geedmrcyu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gqglczsog.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gxmzbiwug.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gmvpsoder.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gltulhhhx.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/goqiktlik.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gadxfhpdm.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grxcloabc.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gmetxwqnz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyuypggis.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gevkzipbb.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/ganbhuqkk.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gdzygihzs.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gtgkxklvq.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gwiwgksfq.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gaxjwudlu.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ghnnxhqyd.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gtjzkgtiu.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gmkeuezcu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/ghlcmuntd.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gjmvbmiyf.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/geakdexqj.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gzvdpwtlb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gwnkizjwm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/geewjnupp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gfhhdqkoa.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gcespumrr.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gmrcngwpz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gaqbzdsiy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gklzepwqc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gkxtccjzl.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gpsdyxorg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gyjaryvkg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gfwlzojgj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gpyfyuqhk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gpgtsnurm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gwdocqdjr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gzuuqfkhr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/ghhquhyjv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gjzmpgyrz.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gncyevivp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/glqmnuccr.sHtML


<!-- 参考信息 -->