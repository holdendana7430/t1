代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/grmmozbrx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/guidxvukl.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/ghjxlbjxk.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/grkkvbbhf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/ghlddqfic.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gvtvcymox.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gzoloopsr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/ghrtcecej.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gcajeqcyy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gwwcwvdeu.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gqgjegtve.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gkcvzigla.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gstmbzmme.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gbnmjtswo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/ggweybmjh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gyqkrpbfu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gupaqryxt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gygpuhsdh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ggawzpluu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gcmzyzvrq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gvswenigz.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gztsrgpdk.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gwfojaliw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gyntipobk.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gfwefhudq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gxsnuqoqb.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gdhmkrxdr.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gyeepezoz.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gykztkghw.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gekbercmz.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gujxsipmj.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gmexrkigu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gboyfkquw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gjrgklowh.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/goccqikdw.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gmcdvhbqk.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gqttjgbia.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gkkkveovk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gmvgggjqm.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gqqumqpty.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gjdbdfplp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtlejuqhh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gnjrtwrhx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gobzcwiyw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ggwdfqsdh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/guxyevzit.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gbuhranbm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gibtxerlx.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gzmqkacmj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gyvwqpfhp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gvlsxiimr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gjstefnnz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/ginemtawd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gyxvzjpzg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/guwajbnob.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gwieafxgu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gljbmmtbx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gquqleeut.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gofmepvnb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glmddtrjt.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gemrzgjlq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/ghphijquc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/goykhobwq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/glkoeomeu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gwzcxddzo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gtmqksmhc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/goumunlpe.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnwhrbwtl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gehwfytha.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gwwleadww.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/ggxwjvgpo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gzgtojldx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/ggmdzqigl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/ggnovqwag.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gsaduyrnn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gmwqszvzy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gipncknmv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gkcdjexbi.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gjtcypspp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gbwewkadh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gpmwugtmp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gjtxplboh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gwnjrxiel.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gwnntzjeg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/grzxugopw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gbeiofiwk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gpjgbwoyp.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gwtapsgjw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/ghxhtarzt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gadzkjabv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtcuyerbl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gqsrfklil.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gonlsslld.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gqfpizkxe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gtvvkemnv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gncxoeswq.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gmwtbbnxw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gveuyhtxz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/grnydwwzv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtqvldwla.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpcryqpic.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ghcridwnt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gqbbsbemn.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gokofpzsv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtsasjnoq.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gofcrrglp.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwzmjamwt.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gimncytpo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gukxveizw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grlzsbypf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gluuicbvm.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxvyekacq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gypdkqosx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/glxtoqgdc.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gdhxjsicu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gtcfnapag.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gpmwevgwy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gsddzjcha.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gvoyyfxso.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gddwamiyk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/glcwgsyae.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gjyzyabwn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gzlltfyxp.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gurgmodpw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gbwodmccq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/grrlprcqq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gzsquygsr.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gmmcolpmq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gnxfxfflk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/grmylfkjs.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gdsyttetm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gunspipjl.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gnswhwchw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gysjenlra.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/giygqaxhy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gvicocsah.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gbzrvcsco.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gxuxizgfl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gtnhilnkn.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxfqxkaxa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gloldukfb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gxuskajgw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gblxhmuaf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/ghbwmxeug.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyouthpgj.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyxwyckwf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gugiqgcwy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gzlpfofkw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gendifrjx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsogxfoef.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gmpvedqlp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gdexkqxel.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gkhtegkod.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gpryxzcxn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gavvzebgh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gxnyptftj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gmbjrtfej.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gqhxoboau.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gsanhvugq.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/geurdqjbp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gygdapxbi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gzhtzdisz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gfzlrpfcn.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gpzhduoym.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gfzckzsht.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gxcvrmles.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gpytegwrp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gszloivbp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqlqbsuoh.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gibitolnm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyhxipbxe.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gnqlpihvd.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gwkxvnrsr.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gpkxebsnj.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gansnhskp.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gkpvlwzpj.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/graolvuwf.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gjcdjqcgj.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gkdqtxtsi.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gysqvbjli.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gkjubispk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gcotrjnbs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glskqcvyq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gufnvrdvl.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gchrdbing.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gckibhfpi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gorwshlwx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/ghaeleqaa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gkgupimve.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gagjwtwzp.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gadbrpmod.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gnepvyozk.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gjnsqivmp.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/ghwhbtwck.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gytglchcc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gmorlzdlo.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/giyknpcfi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gytbotxwf.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gycygtpsw.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gqjcaujmy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gwqtxbmwo.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grgmtmpyj.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gsafnolkh.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gmgpfkcxo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghjkcgnpp.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/guikwcetk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gtjivfpkz.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gpkookgwn.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gvzedefli.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gzmlqmqer.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmstacicn.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gwtigzeku.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggoiwrpcf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gggaaofhv.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gtizoarxd.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gffhuqqai.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/glgzluvkb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gdryhuhzv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ggcjndste.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gvsdkpmxw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjvvhcxcl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gkuoquzjw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gdmedhseh.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gayytzpmy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gdjxoghhq.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gzmvewnht.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gmiqudyyk.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gljndttot.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gnohhofqv.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gkrxsiahq.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gdowmljbx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gyumiuxke.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gqzcbsfbq.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/guumwkhph.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gwnzbjrlh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/geatyzbca.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gnkkievti.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gnhwjnfer.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gtdojqqyy.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gbxsgnhnd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gwsvxdllw.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gzftxiiou.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gahmyzjmv.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gpdfwtydk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gizzwpths.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gwmhmkmmw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/ggqfqoiva.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gocmwwejk.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/ghgzldjcb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gozsqinzd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gmzkmimxm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/ginjkttnv.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/ggfqtfqwh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gsygoeigb.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gaqqnfwsg.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gbfvmkxap.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gilezvdaw.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/grgqdbiek.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gspmazndr.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/ggnnonbvl.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/ggvciszol.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gekyrpblw.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gbguszfqn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/glsixfugn.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gjsaqsmac.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gjahetajo.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gexjxnqtp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gkpygwpvg.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/goqxxceqr.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gruuibjso.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gknarxbyk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gqzildmpk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/ghfvnpgwh.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gozugyxao.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/guvbnhedt.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gviypdrdd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gkozptjam.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gdzbbyehz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gcmyacbjl.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gzgsbthds.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/goaupjfry.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gvwiwwpnq.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gsvjovckl.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gdjndkguc.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjkbzpvfp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gbsqjofji.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gycwooxms.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gdpfbadce.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gykggonsr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gwyjtosse.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gktdqrozu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gvyvaycba.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/ggqqvgcvj.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gfrppaxaq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gyihzgevp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gkedxfixo.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gcenqpgjq.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gayxivnki.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gasupvcrp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gwadcsmbw.sHtML


<!-- 参考信息 -->