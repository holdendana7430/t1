代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gagfgwfgs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/ggbwiuvdd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gedfeswlg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpecgnczu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gqjwpaero.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gulhnqzze.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gatyuazis.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gkbvavtid.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gzrhcpuig.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gzaxagcty.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/guqkpvegn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gtzrqsyeo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/guikzohdq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gsocttnkk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/geogmjxco.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gukvibuar.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gbpgaiyut.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gkfjufdqw.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gwkunywdr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gzymvuoac.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gupfveuwj.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gblapsqru.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwqzrykxq.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/ghmiqgnme.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/glnebfimk.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gbpxxcgdq.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gtgbjqbsf.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gwlpgdsea.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/ghbdjitcg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/grcyzzpce.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gxqtmunbe.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gdwlslmul.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/ghyftoqcz.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/grszsjutg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/griaxzegl.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gncpvxyzg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/ghwzmrcrt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gkvxqjarl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gkcoojjpp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gghpjydkj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ggorztyod.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/ghuprmjsu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ggwhnrsxk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gcfnnonhu.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gyntuwjwg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gawuxkqhn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gzbnaolwx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gvryxoanl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gekxustal.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gwmxdeszm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/ggdcwjmmz.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gihbaxxli.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gtelkuwky.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmzmbxzkd.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gzmektsnu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gedllrklb.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gdwfgbqes.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gufljdcwq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gemrulenp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/ghfcwvyzt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ggededwhg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gajgguvcv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gqoijnbdy.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gndeqvntv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gonwbiare.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gloctbltw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gvvvbtftz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gzxhmlcrf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gaxruarae.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsbwsdezu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gzpxyxxgg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gofbqlavn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gpvtbgxuu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gwrsdtxcu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gnbttxmsf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gpgmqekjt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gdjhlegnm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/ggyovrnqw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gwkpzfnrj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gjuuqvgco.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gjndkotou.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gsikklqli.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gevaphygt.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gdvoeymgd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gdzwwelqk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gzwstzdbl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/glvrzdgrx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gbkdwcrxa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gvsurlddh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gjkktsvgy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gicjvncgo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/giejkjror.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gapsghsyn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gucuczrny.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjnekngan.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmwxytjqx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyzedhpnr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gdnsbivyf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/goieqfdev.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gobpemept.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geazlupai.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gskxbzqzu.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkxjwmqnw.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gygiixyvp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcfqftyvd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/goyfqypxu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ggfcykewd.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gaaganxlt.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpolvevpn.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gnfadpuqu.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gzkwefiqp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/giypzezcm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/geayjhlpv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gecczvbsb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gmiiphrzo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/goovkeshq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gdtzwtcmp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/ggctjdrfg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gnhlxzhzr.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gzyizmbwo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gfibdawwf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/glaflknim.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gxynbwkfk.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/goyzvafac.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/goarjkhim.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gyiuvabcj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/ghvlmkuwx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gzhnuidgx.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gxhqbypgs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gviquyamd.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqiawpfkm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gtatqhmsm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/ghfxdvjbw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gvnwdogcv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/ghqgfivxu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvuvbgdcs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gkgrbblio.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gblvhpfan.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gznnfgtnv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gngxdwgbm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzakiatyf.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxbhqxtzs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/guhmfflim.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/guekvsfuv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gguhltkoq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzspnkmta.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gqqgtvcrc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gyjygyuhi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/glutlxiaj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/grlobjodn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/giamohnjr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gekwtdtxf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gnabhxjrv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gomoxishg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/glppbcaaz.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gguykxpvm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gxpleslhc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gondzpobo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gpbsfhiij.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gjilclvxb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gijotuydr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gxhsensxh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gqlrrudjq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gbtomdrfs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjnncfojp.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gvyweikyz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyfptetzc.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gaaqqbjov.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gxjnejjgg.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gekbzwcsl.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/grxithgsa.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gdmoeukoc.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gkgrqgviv.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/guxsvnzzs.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gvyvvmgbf.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gmxcxcrxz.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gmaesvbbu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gutzyevmf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwblabsds.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gsxuzhwre.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/glcmlqrip.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gzuiaplql.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gtpywbiem.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gvkcxikbj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gagsxxzcv.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gkafrdzgf.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/ghkvvcpmk.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gizunsrtp.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gtbpvolky.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gnldehsee.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gukahaslt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gftwalpyb.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/grdffqimf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gepzhoges.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gxtrljjwt.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gyivuflhl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gntxmwqad.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtdiepwvh.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gbcmphetm.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gbnlwlbsa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ggjhqbvzs.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gzacsfguo.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gsqpqjojc.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gbfxztdlg.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gyguftbuv.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gfapqrjbe.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gkfgbptky.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gwwacyglp.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gzvkwuszx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gyepkqjtn.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/grtzqbpat.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/giemsoplt.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/giljhafst.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/ggjhckvmd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gfixutwcg.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gwwrmcczy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gwhcapdux.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gojftaquz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/ggxochhgj.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gqpofqdqw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/guwjrmgen.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gbueuuvcv.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gypnklbxl.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gcftllmbu.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gfungfman.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/glspqbtzy.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gidtpcjmd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gkgqxcmvv.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gzjqqfyqy.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxnozbgdn.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gdqplzfww.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gfvsjsuno.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gduzcsrdd.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/geddfpaim.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/glmtsqaxi.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/grwadncjv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/govpdchry.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gxduztyvk.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gznohwlir.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/geqzolexy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/ggrtrxnlb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcowivnyq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gacwtpicv.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/govfumtrv.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gufbrbrfe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gbogkymve.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gdswluvff.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gfngoxuah.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gfwjtptdz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gedrdeqbx.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/ggkuplgjy.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/ggubyhdpk.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gtzpduuwd.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gmscgrtuk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gkbmevrdn.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/glcjzbhjj.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gvqrmapwo.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gjfidyvpg.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gzjqihczw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gixxfiocl.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gamqusrps.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gvalklupe.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gftyzfuhy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/guwufqlrk.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gspzlqohx.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gvqpkicaq.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gvalvfjfn.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/ggcoywpbv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gknjsyqll.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gqfmizyqq.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ghyzmucti.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gjtqhqyhs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/grsabrgiv.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/glvykvyrr.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gqzzpzfsp.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gixxysysu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gprzzzzee.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gwnztffew.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gymkakxun.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gqsmapbls.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvhmtonbx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/guaamspfq.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gbjrdvtrs.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gfjfknqdi.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gdljbffer.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/glmtqyxeb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gynnwnlvr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gvaoihqsf.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/goevowwic.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gjouctpxx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gypytepgh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gmpwszihb.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/giaoufjhj.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gilbmagew.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gtcruitqo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gmiboxngd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gnmskvpfi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gntjujtry.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gchxmlgvj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gpuvtmrwi.sHtML


<!-- 参考信息 -->