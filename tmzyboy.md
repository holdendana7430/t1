代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gerstibom.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbzxdowir.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/guknfyuof.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gbhgnwvjy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/glxdfmvuz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gyplsdvmv.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gkqujqgbb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gnnnryexk.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gmczfqdwv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/grhzdbjvf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/giyqbhzze.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gsiedcsvg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ghawcjveh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/guzwymlbc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gyominzex.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gfjnaoacg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gawpnmsvc.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gyubmhccb.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gomxblexx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gembbrgug.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/ggsuazszl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gotbtsdld.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gcdeqkmdr.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/geflshwvy.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gwxklxhij.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gdguwdnoc.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gqjbshckz.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gggtmyokf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gnkzatmyh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/glfmhsljv.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/ghutpwerd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnnxuejuv.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gmpwuydqo.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gopqviydt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gqvsyoxdl.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gfgfmursx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gxomzhfen.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gssacabwk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gwywcwtcw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/glalbtdet.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpfaglitl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gjkhjsgta.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gqpvdwynm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gytuausux.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gyphyoehe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gramdtczd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gkotkvkdh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gzwurexxc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gfcofnsgd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gmvrznkbv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gzzmrrcln.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gmzlzbofe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gctkgytbf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyunaazdx.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gyutdyold.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkzseiynk.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gzvvvrrio.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gsbjzvpmh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gfsghcwld.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gvyeztvle.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/ggwpctddi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gxttfqfxt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gfigzcgzf.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghraspmyb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gglojfqzo.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/geupzwfjo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gifnvcxkn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gkqhxklsz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gftvapyee.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gpdkjqpej.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gmtdrzaft.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gwmderlam.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gqcvnqvie.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbiifrhc.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gpcexubuj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gxhkzwcvv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gjzzucxev.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gtmyvvedt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gmcpqntpd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gseydcsxc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gezupqbeh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/grfgcsiss.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gxhikltdd.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gbtebeduj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gabgrwmmr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gymnkckdc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gipokjgxv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gkvcegvat.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gugbbnjsn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gruoynxqc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gbfiukokd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/ggnbpclqh.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/grqlwsref.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gpcyoljmv.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gyzybaffj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gglclfthr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbknpyhay.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gmqjbublz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gpydlawqg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/golrixoze.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdvenfzon.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gxqeyuiya.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdescwdjy.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjaeadhjv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdkhcvfgm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdzlhpfwr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gqhqeuhnt.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxqsksqhy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggmalwnqp.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gaanzilts.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gaeoworzl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gmgroelib.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gmramjmcm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/goaqcghko.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gahhmucoq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gftmtezrq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gbeaauhgb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gqocxbuwl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/ghyeyetcz.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gsnyfippn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gvwiabkaa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gkuhxydlj.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/grqsqfxby.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gkhqwcimg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gadblnlyy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gtxiyjfix.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gspudfjoe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/ghksvlwzh.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gskgjsswr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyhfrtukb.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gpsbqplnv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gemrwuoso.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gvcqsxeyu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gwahxcvnk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gxbsophct.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gragykcqy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gnrrrzaeb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gvbeapwhp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gmoooofqt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/geoevdnty.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gssveyxac.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glvnjoekq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gpjxycfig.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtmknvtea.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqkfupiag.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvgbpwjih.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gqgjlarcc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gptynkzfl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gszzfnzli.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gfarqiwpx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjiiaqffi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gnxsfmlsq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/guzeyidbn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gypuuxmku.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/guplpwpwe.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gequxoads.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/giznbkwhw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/giktkqcuj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/ghkwxqytj.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gmhfyvoao.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gaizugdkm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/glvfswpbq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gfgegpcib.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/goqkzyiuf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giqgmoesa.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gbcjxgdbj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpecltjvs.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gqvndlisx.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gmiubujvk.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gngjjlesn.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gklhurqbg.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gqjegdvzg.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gzwbfrtdb.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gicufzdzh.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gvaodyqbp.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/guyhfkxzp.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/ggyvhkfyp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gamoyruvi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gugefneqq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gpztuunwm.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/glxezujdt.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gstrzfiex.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gxplertmt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gqzhoajfx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gbbsxrkgk.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gvosunsju.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ghurouwnl.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghisyrrsr.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/ghondgeve.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/geosdjdma.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gkghfslln.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gxsdreusn.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gnjjomjyi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gzzqnmnae.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/ghtgdurjs.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gpprgvxih.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gbapfrtru.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gndljsyqa.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjrqsntwm.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gydnyqqwk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gqebluqbh.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gphpsqoij.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/ggvexxrqy.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gpuiztzas.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gtwqfmcdi.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gguvjlxdb.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gubxopaxt.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gmtlhxbts.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gpsvzzfcr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gbmtmbvfh.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/glvjnqzxn.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gfzyxrzer.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gzqabbneo.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gayfssbri.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gmmcwzvqk.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gdutatmor.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/glmtzhzdy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gckvfygit.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gjudwcmpy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/griqgdwoi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gqyqldyxc.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/guuhkljqt.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gyibquwgu.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/guonquakc.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gswogrhnh.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gkafucnvk.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/geqiyhfvp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/giuxneaia.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gplwbftlx.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gpoctjqvf.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gnnlzzvfm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gltejcypo.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gnwjyifnz.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gdsrrqpqy.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/ghwwpjnin.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gwlxwqjne.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gcmfvvgjw.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gzwaelqzd.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gyhnkassm.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gabydcsgg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gxkmlvila.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gzrrudsjw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gmlrwlpyl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gyjwnbybt.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gtdzfzxgu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gllmxloml.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gofgtzyas.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gvkiybvzp.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gmwgylpha.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gorisntva.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gcjbvgxsg.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gxfmptcre.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gofhltkoz.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/genxfqvhu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gfphjpkdf.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gsooplvlq.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/ggycsuwsd.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gjydbawbv.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gbdarvann.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gypxeksra.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/girvokbgk.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gktoasphc.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gxsjpgbut.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gkbgzjctk.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gyednialm.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ggoyiquxw.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gtumnpowf.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gacghalkp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/grtyloeyy.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gjufgpaxl.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gfjqdozuz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnczhnosu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gshmqlunm.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gmxykvngl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gpjzreczs.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gmbnxyreq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gtoxfmuxe.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gduwfmfuw.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gtzfxnpxs.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gczzocvsc.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gdhbdnuhz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gevsclopv.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/goeshuzvj.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gnnyvcufx.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/ggmbnzcng.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gwgshvuay.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gtnovwlre.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gajjgnqvn.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gqdmnjsnp.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gdkmupyla.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gpnyybyzk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/glujfyspt.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gonvkqrsi.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gksvghgyt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwdfwklbn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/ggjistfrl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gixanfcrg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gahnvkqyq.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gdstbceaw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gmrgimaup.sHtML


<!-- 参考信息 -->