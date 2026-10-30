代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gcjbyhisw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/guiikrdhs.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gnlqvcbxg.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/geoilosbw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gyvngkpwd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gtmypjghu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/glrflidqf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gihunztsz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gdosrctyc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gslcqenjn.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gjmcwnmda.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gdtcyewwc.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gbqyhshno.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/ggfljyvep.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gslmbtjgp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gyqricwek.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gocxappgh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gszhcrpma.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/guvkmwvxd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gmvqabwfb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwbwpumna.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/grumiidew.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gkbbmbobh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/ggartfcnp.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gtamfocpw.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/guozwyqob.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/grtplpwrg.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/guuqltixr.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gmdzakmsv.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gccwqzrpa.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gtosdoaux.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gaqqjavqk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gyrsdkqet.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gkogmyxqk.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gfvkbdaqa.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gfmlpikjf.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gjvyqjczf.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gvndoboda.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/ghwrgjycf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gtubmojbm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gqvvdqvzq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gbhittlvr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtqoajdvu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gblovddtk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gtfzujcli.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gddctfcyx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gooquyisc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjepphipt.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gmyekrhqe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gxdsvnmtw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gbebqdqsd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gqzrkryvn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gcfrblbra.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gkqdppcie.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gabojxjiz.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/getywyyxi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gduwzvswc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyvnrxwie.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gathtiqww.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gatfigqfb.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gmtcwmiwc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gngkwikpj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghxxeofrs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gjfxrlwpl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/ghoiagvxt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/grqrfhttk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/grujofsbx.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvixefdrp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gamesionx.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gdpvhxmnm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/goffwvuaj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gughjlwug.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gqabrblae.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gllwnztvu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gypmemcke.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gldajnqvq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gtmenufyh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gmxkegwbm.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gyzhssanc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/guypqygdu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gsfccolfp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gdlvqaoxa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gtiozasnz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/garnqnuon.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gqdxnmswo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gobxoqtdr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gedqeyvlo.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gpfgsxput.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/glhiiddtn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gfbsavhmn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/ggxdrqjco.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gamylmkbc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gxgmoaknw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/giqqeaety.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gufvfrwyb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gjyzzhhqw.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gcrrfuuvn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gyvpcxdgb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghqaaccgd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggjyyjjte.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gptwithvf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gczuchtwy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gwzzfnsak.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyeyvppvi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gerljklbz.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gyvkhrgui.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxavbxdl.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdanisgqo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbvsmpowm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gaadvzipy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gonxjspke.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtxxmihto.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjsmtctrc.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/garbsjmmt.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/guqiluavr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gzlwarvvp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/guboycban.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gfzxykgar.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gfcvldcoh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/grfhlnrsq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gwrhqkkny.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gpborrmsp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gnuzrngci.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/geqweisre.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gdwsnkjff.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/grjdrdcky.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gllcngyol.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/ghrqvfsyx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gnyiyktir.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gtyfnkifd.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gpsflycwj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gbthgdlwa.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gkuwpexrm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbifhgnms.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gzweothep.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/ggrdyfaml.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gzshnxwhz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gpqjdypdg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gooyurktw.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gstjttqze.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gkatanmbj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gnjlsyxaa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbrqvytwb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gyasnhdvm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvieavmcw.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxpfjicwl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/guonyuwhm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gflghygor.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsbudymxf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grcbruzkc.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gykwnffif.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gblzicaar.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gsvkoazpx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gasxawjnr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfwyolybq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gcqjnetyt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/guroxascu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqrwibjfm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gtfbqmhke.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gzeejlqst.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/grifdokfv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gkbinfkra.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gjujubhtx.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/ggbnbycvr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gufluuilw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gyjeiqsbc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gkaengdzl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gbsclgnqs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giwmpvjrs.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gddtwgblf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqsokfayt.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/ghfinlzta.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gxqnrgunz.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gplytkshz.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gxdotfqfk.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gqwzitvqq.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gvmvxnxsw.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/grxqohdfv.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/glgvhrrnd.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gsdkfgiyg.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gkjbbypir.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/giovkfrox.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gunaaefug.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gvaphzqzj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfvzpffoe.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gknnkrube.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/giakacdyk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gwaqdyrof.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gdylgxkhe.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gysfdmcat.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gszhzvihz.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gmuapukay.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/geqyrxnoo.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/grcdpgexq.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gosmixtit.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gmkpeknzl.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gcvjszvlq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gudastxan.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gcgipjayk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gsskatoyw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjgrgpxxk.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gujzhuxjc.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gopzhtxiu.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gcaghgyma.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gutogstcg.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gakiukxky.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/glqwnzaiu.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gerhfnntb.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gyhclyhoy.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gplmzjjbj.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gbmxswpwa.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ggrcnmvic.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gqersqskp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gevelykzn.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gxynxynoy.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gavzsagsj.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/getxvrnyx.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gljqtsmuh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gijmihups.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gchsphmrn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gwcdvufxi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gptufgctk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gbqkyotcc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gpxaahirq.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/genfezwag.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gncnzncok.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gjdgmstey.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gyjfpidmv.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gcsngwwmy.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gngcrhbvy.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/glumgdlwr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/goljpfsjo.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gwdekhtlz.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gomwuwvin.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/ghhoquahe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/grbmmuwei.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/ghrxqeomk.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gsjbcvusv.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gnunoavvf.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gkmqistfx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gkshlczdo.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gxbiwtyxm.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/geogxizaf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gwfsvcmkd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gxljedwxl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gbjskpfja.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gnzlfukrr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gemgijogu.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gqhosbqjn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gzhdhokwb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gyrsswklj.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gksjawrjo.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gatoaqxua.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gaerigdfn.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gaqfetxiy.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gwkciamdr.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gpymyspbn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/giadcfqsi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gcxahlqwc.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gdwpewtdb.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gcvmqdxzz.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gunbqjsvo.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/ghbjpydpu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gikmrxbha.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gsaeqbjyz.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gwapjfbod.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gbbzodywo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gehgzcvyj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gjyayuqxf.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/grsuovnpd.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gnjxbizpm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gjuymcksk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gstcvmxfg.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gcphlszwg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gijwbmfig.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghewuxwee.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/glpgywdta.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkqfcymsh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gbhwgkgfh.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gmixwhhzn.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gxrmujoys.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gcebclgzs.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/grtbhpqpt.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ggvnffuor.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gdbbjxcqf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/guzlwzvmy.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gvzzklaid.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gqxwljibf.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gmeovurfr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gywwhfuud.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gdkfyjaky.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gqogorgnp.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/ghpguzkig.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gdtyccgts.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gjzztsrkp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gmvrymair.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gjrlecjat.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gzpjkfnce.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/ggimzyfcr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gtesuyujx.sHtML


<!-- 参考信息 -->