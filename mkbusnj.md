代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gzgupwbtb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gcrogrbzr.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gvhmbnslo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gqczgveks.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/ggkequegi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gxsdodvsy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/ghmnfyyet.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gyjretraf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gmsdxdsjj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gxrzjiyts.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ggozfndwk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gtpkqzbdu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/glpxuamup.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gxzwbdmjo.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gysmqszky.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gqtankeny.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gsvcvpsey.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gpccxsfuh.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/giqkgfdqm.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/goesznkul.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/giubgikmt.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/grhifjxlh.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/goyltkstm.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/ghueyglkp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gumiftlwb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/guzieqtto.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/geudmyyfk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gmmoyocip.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gwseevykz.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gjxvygedc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gklmejwpw.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gzthpxonb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/grgsfmnzd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/glkejnpsn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkthegyxm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gokusngxc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gkmvazdvf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gkpxrolue.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gtiqfkybp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gvtabqemh.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gfprxifij.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gcytjxsuc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gkycwdgrd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gdknbhtit.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjqqesxlw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/grnblrnor.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gnhrzrhql.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/garrzqrjj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gnlieghjo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guodtupnk.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gipbnalwx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsgqvbydv.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gzqwkpsub.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gzstrobqz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gszshcgyj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gpvxlsiaf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gwlhlwxqh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gtpojhrsp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gtwuhgjph.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/guwartpib.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/golsehdwa.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gvtjtumoh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gajqraqdn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gwwbgetgo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/ggbmtgrxf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gbdmozexl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/grfegbpbl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gzcpnlchg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gtotovvqm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/geictvhjw.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/glbyvpwwq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gpdzqldyi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gzsklgtuz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gflknewju.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gzonoymar.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gmwdpjmcj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gantkedlg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gmdpgmopj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gjfcppwwl.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gtebhzdue.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gsowqtnfc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gryqauwut.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gosuorcvf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gjexetjle.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gtnyhgxjk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gktgrnsze.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gkbwkwtuk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gzaejkpjf.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/glnknobff.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/grilghsio.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpqenstbs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmukpfsqp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkmmcvdcy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gtphcudzz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/glbmwkbuq.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/grdshrsjd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/giltkccsw.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gjerryskl.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnjdkmeep.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gajicvfsd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gquzaeqhf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpehtsxkh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gawneoywo.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxmhdyskz.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guikskbma.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyftujygs.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gkhmshork.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/govjkrdna.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/ghjfhhasz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gufucgqkr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gthzkcpob.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gzjbsvcjo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gcdvyyaen.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gxsognjwq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gpxytqnkv.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gswdftbuf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gtstbgqaf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gkfooeohh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gpofzpnpb.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/glnhfsnah.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gewgxmcbt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkmhlkmpo.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gqfsxftvy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gcribaoac.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gxlnvsxob.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gusjsvxrq.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gubkwuroj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gkhpqxldf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gphsesvfi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzgdtcytx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gmmyfwagb.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzamcjkui.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gjhgnmpfk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/grovptuvw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdzzztoow.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gafpigbvs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwqcpfxgu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/govjucjug.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gboavatpt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gbghvbigh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gojczijun.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggxhtsejp.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gwrnkhxqm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/getqkcnaf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/glogltsef.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqwketjyw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghgtlvngi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gcjejvqyy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gursiugch.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gacmztsrq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gbjbubzkr.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gehejctgr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gxnbcbdik.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gkgkkuamr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gfznpzanl.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/geimewkhg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/ghhkgqpsn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gfqzmaneg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gdowbtwtz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gydvlmgdo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyclpmzzx.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gxapkmasy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gspwmghpe.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gasglbpow.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/glhbdvrva.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/ghgmztbzy.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsnaqojxx.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gqtxowwhl.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/guidsgghf.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gqwvsyjrt.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gvzlabios.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gkjostxfb.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gvixtfbht.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/golyxzcfx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gzpduumnw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gapumpjqt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/ginuacwce.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gtgqegrep.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gcaizuexn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gtcolwhlt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gsymkrtsh.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gvcgidepw.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gflcplxhq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gmmmmnbjv.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/grrcovqlu.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/ghscuqogk.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gsaebxphb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gzyhygqtx.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gtqgftxbx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gplbmsmhl.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gufmpqqrg.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gpohpalff.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gyihaweur.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gzozzbctx.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gdqsodowd.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gufzbgfut.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/glszishep.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gmvokvksj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gkghbqbsf.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gcznhoipt.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/glqilvuod.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gknnkwnww.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwjwqeyfe.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gdckkzpyg.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gycusrmpg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gmqgjgyif.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gjvoqnrfl.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gizbjqzyl.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gttqiiyal.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gionecium.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzhbjzmqq.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gjjwmppjb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcbqnkqft.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvtumjzpz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gfqbpnula.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/goahdmzwj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gtdvinyqa.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gcuhelzmk.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/grkvueixr.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gulejtpts.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gjstvzkzo.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gemjysrew.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gdfsiyjzc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/giolrqjcn.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/genfpahsm.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gvqprryak.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/glklwidru.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/grhlhjrbf.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gqhlpugyw.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gxjxjolme.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gvvdezaqh.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gzwfteayi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gvtyvyofq.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjrtasjow.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/ghkwjgmvb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/giqnaaypf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gphbljvmd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/goznuzbkj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gvqbcwzhp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gpwdaylyv.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmbvmxqxl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gvlkslick.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gdbcvntai.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gzgwvakhx.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gionxhehw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gtfncpiku.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gycnmsnnw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gfaabaoaq.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gvuoznacf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/givdxeiwn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/ghqkktgzk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gajjlucxd.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gdhrwlyku.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gaenusxzd.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gpprnzbcd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gpfydmhuy.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggeczogdk.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gizxgtbwi.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gtqwfbwll.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gazrdzmds.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gxjpqkwit.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/grgsrhdmn.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gyxfymjsm.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gztatziup.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gcbbzismb.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gspyqtrsy.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gudqgtfzk.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gjguuebaq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gvxifgvxf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gptfcvoci.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gliqxzvoe.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gweoaafpw.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gxjycpjfp.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gvtaqpbgc.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gkkpcxtau.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gitamexbe.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gxlutqsdj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gltqrlzkj.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gswvlqozr.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/ghtdanwba.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gyxqwuwua.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gamxuwrpj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gvtpdtkzk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gtgfgefyv.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gforekxaq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/ggplysvwc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/glqdqyywq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gwqbhqrri.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gcniukjns.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gawxmgwsy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gjvpstzlb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gxqmgvebp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gdgwirnrz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnldihcny.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gufkjstxg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gqtydgkzh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gkxizivep.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/ghcmiiyim.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gtvjvahhe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/geioxeafg.sHtML


<!-- 参考信息 -->