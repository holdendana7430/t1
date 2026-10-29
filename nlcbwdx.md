代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gyvbrpsdi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gpgcieawv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gboyakxjy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gdvvfvmej.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gmuvaeogt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gjlqgowis.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/grnnzyrfs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gyuleyjir.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gxmrganwk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gvkvtejdx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gzysaozww.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/guulfiiky.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/grchniffs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/grjuqixxn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gkzwhaqlc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gbynphuss.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gphhmrtsj.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gesbiaotj.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/glnghfmga.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/goyuntrvm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gxjqodkfb.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gqjtbrwgc.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gtixvassb.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gdusyfasg.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gsumdllvf.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gpwpbydzf.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gxwlbdgjm.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/grwpgjnee.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/grjnlzxnq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gacglogpf.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gtegyhqjk.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gjhrnrixg.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gmjveheqe.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gkyitxzbu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gloszujli.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gfmgmzlve.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gcmggxnpi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/golkugxhd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/guudnvmap.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gujaqyhqf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gibsjcfqm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/golzahjvv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gqlnstvgp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ggbxxpomk.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/ghngocxgl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gubvqkbkp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gixtjjntw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gjmslndpv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gimwspvbx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/ggqosrzff.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gmsgmgrik.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gotmnhgad.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gvubulyrg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwldtnuev.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gpycoriup.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwncbusvl.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gzjrflsnp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/groftnwxw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghmmewlsj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gqyxdkgjm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gzchamrze.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggudlnlma.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/goemtgysn.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzbhaaxro.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdrlmxlte.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/ghsumsonl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gnkdydkye.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gtncfywif.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gnnqkbwek.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gxcsbxuiu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gcyrjucez.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gyouwmleo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gfvshbfah.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gnlmayvrh.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/grqeeteib.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gfznsgxbz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gkxkmqqlk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/guoefpbzu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gsbjftybm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gyhptlbnv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gvodoeofz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gbgxswsys.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gbjswdkpz.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gebtrlajk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gnjmuhekg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gyoffnzzz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gdrjanzuu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gesasvqjy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gutzcifsm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gxceozhhs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gnwyeefrx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gptkrrafj.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/giovxzwlz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/glqyondwf.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gvzrfojoy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grcpmjost.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/grztizzdx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gqftzycbs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gxvljgzzz.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/girfnileo.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfvyzylbb.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gcrbshjdm.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcdurxcsd.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwssglymm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyinfkssb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvxazvtzl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/glrdypxqe.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwkoxizbq.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guzdzvngm.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gscbuvybb.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gxnrneutd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gflxaleva.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gdefzrleh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/genyzpcdr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gvbpcnkyv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/glwpziklw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gajyqdszi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gxmetotif.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/ggkfzusfm.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/grjdvskid.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/glskukqza.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gsfdkddst.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gilscgjee.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gsklegxje.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gjmowqepe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gxqbilvif.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gcooudojn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gwhvcbvqw.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gaevmgzxg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpozjzydv.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/grelmwekj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gvatvkpri.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gwojcbbkb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/glhqkmspq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gdrmbqtrf.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghspzezuy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gfhcoavkh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gqygxmxvn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/galjepnje.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gquniheae.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnggtesey.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gainfiona.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gcheavhvn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcmmpyzop.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdaskqdnm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxbimkims.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gbtyumaem.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsqvpxnkj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gsuebrkxy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnekmvfsk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gejdbyplo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gjruaogra.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/ghopeshhy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/genzlknml.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gxsrtzcit.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gihbygjpv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gjhreppaj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gcbaghowz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gfmcnwzok.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gthsgboyg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/giuzunrcl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gesxyleue.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gmrvynxru.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/grfpahikr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsflliqwb.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gukznvesz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gywppxzid.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gvomtukpn.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/ggyyytlti.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gzkknmsgo.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/goxkvcivl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvaktiis.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gvgaeoyun.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gzjhijftw.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gppbaiolw.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gmtxmvigg.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/geiyiuuor.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gmvwpqcag.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gxmmohasp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/givpxdfap.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gsznrbxaa.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/ghqemhpae.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gjbuhfkdt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gmmksytba.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gojxmzqtl.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/giquyfgom.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/ghuxtdipv.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/ggwefqpfj.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/glilbtfng.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/ganpsqnbv.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gnzzavvdd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gizziwtvm.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gopagostb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gtsbvhair.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/glpzmltdh.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gnirqmuvv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/golofknqj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gkcpljyid.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gwybqbokt.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glwrmlmfo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ghlvcbghy.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gmpyshmxn.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/giarfafrl.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gfozanjhy.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/girqbslmo.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gugmzpfyz.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/glirpznuc.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gtfudnxru.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gxfwbytpx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gcoohwlbw.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gmibkxddk.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gktgwqizh.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gdjydxrpk.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gjxgesnlm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gnghjxtvq.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/ggrfmlzor.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ggkfdcpgs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gbpfjcjha.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gpmwppsma.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gjiyrjoht.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gofxqnyci.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gqmquunwr.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gloebghxd.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqdicfpqz.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gzudqxksm.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gtqdktkpz.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gmttfgzka.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/glfmtdzhj.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/grlagqtow.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gmvzpzawq.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gbhhwrzpa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gxpqqxxpm.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gnmdtbehx.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gjpsntowj.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gahyecntt.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gfslwclct.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gisdlswyn.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gfilbadws.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gupcduool.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gmszvxeih.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gcvvxutkr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gnhbrdcqh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gxkrxmhlf.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/genyrwhij.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gnsttxdwb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gqaxsxbha.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gmqychoga.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gybgoiird.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gzmdgrtsd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gixqljzlm.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gvunlfwja.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gykuldmvw.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/glxeezmgd.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gjtpotqll.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/grpygkuwl.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gwoarpoef.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gldydiahy.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gnvdnrqwa.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gsbmmnvzp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gtoaiygjv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gryukylyu.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gxriibkfo.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gpbkcnllk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzrmyqxri.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gjzjhdhao.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gahvgejlu.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gcecbwqko.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gyjezgszr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gtmzketrz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtelpwfdg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gybdxexrc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ghcgoayav.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gbhtdcclj.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/grghvqokx.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gykfdgxjj.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/guheejbye.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gubvowqvh.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gpjsyqbey.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gagbehaid.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/griymoaoa.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/ggyhhaubd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gmaeyrbis.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gyeoduuxd.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gnbgdlxkt.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/guvpydgpb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gyflkvpbw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/grzxtmjfq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/ghvmprljp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gbqzzdblb.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gthxpkjip.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gqrtdljos.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/grkbvyxuw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gaphpfgnw.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/glvrkkfct.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gujexfnto.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gbnbtaxhi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gevsuzchm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gbrdskzsd.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gyqlfcjpq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gojmvkyyh.sHtML


<!-- 参考信息 -->