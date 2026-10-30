代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gxtokngow.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gdgosrjgi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gfvaffcnk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gxwcejsgd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gzfpjvckt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gvtgjnvhq.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gllnopicr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gapmlgtnb.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gfmfftdte.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gmkuptdpf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gfhwexdaf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gvudxeohr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gxvxsuecz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gauoqgxxk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gzkrwvlwv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gccipsopu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/glyiabmaf.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gohwjusis.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gztfqoqhg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gbsqfrlqo.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gycmoouey.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gcgauxdsu.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/goniqimcp.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/giolowsyk.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gywiyowtu.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gejbgqywq.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gklvuycbf.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gdhtzgjia.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gyttdrgqw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gziicqesp.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gmmjqxwts.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwgwvyujy.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gasaraltl.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gqzprglib.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gflfqsxoj.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gajjlqapn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gezvgmdyi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/glscqjclz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gcihcgnyz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ginlqoixf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gemotupvd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gvobryihe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gzhwtcxic.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gqopetihq.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/ghdwbwwgh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gytlbhjrt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gpinxzioo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gzglmfqgt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gheloebmz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gsushishv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gbkxompky.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/glhggruiz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/guqyxsjfk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gggwawzea.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gyhpzmsme.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmwgjzszr.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gpvcikzkf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gphyftdhi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfzoupqbj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gckdnlmun.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gdqeliqft.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gtaapsebu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/grhklllyg.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/grojpahgp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtuqbtzvx.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gystdzauc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gehdvjyrw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/glglpkriz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/ghsljwxzs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gzyievsbp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gfprvjcnv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gyatsxapb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gpymctxor.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gsuwzmfym.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gkwtflxsm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gazybzedz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gqpinhrmc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gzumfeyam.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gtdrseyfb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gyjhidylx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gatrjtpzm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gjluekjbi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gyqgdvtnr.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/goujupoee.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gvrrcdxoc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gplqslgve.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gzqpererp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gxicvhpiw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gxurgfrnk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gfmjlsrms.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/goijzqqap.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gxydvjdlv.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gduiwamal.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gmktxsxch.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/guyvdaqma.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gketoqyvq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxlpsldcj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gyyhgasib.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gpvsekpzb.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gprqtlfar.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfadmhjht.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gnrnlhzvv.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtlfnzajz.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gauyepyou.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpmgouaom.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqcdbufls.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ghnztshzd.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghyzmiwsa.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqbaeqnzv.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnlvcpwyz.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/goekupnnh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gjofuvnqc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gpcdxwtwb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/ghbzfnjuy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gogfiqlpa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gaxgsmmea.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/grzynbyjy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gkpgxygde.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gzwqcitep.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gmqdrisbz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gnjxiuooh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gsxtzihni.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/ghaflpusd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gfqjpjgmb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gunpkpori.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gforsimhc.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gbwybtzjm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/guemybdiy.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gijyftfjq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzkqaeqpr.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gopjilayq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gvqtqwoat.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gfvkkkwkw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gxmqjbwpd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gbtnnkzbf.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwnsxfuro.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/ghrasujbg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/ghmmcyecs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxlchiqpy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gpciwixok.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gjyzvjpar.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/geyvcztfh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gjgtinnjb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/grbnuwdsq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmnikvzhy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goiifehym.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gexevnati.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gepuxgbkx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gmaxxqqcz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gvaiqncwv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gmqfaiujd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gjmyyysgi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gyhajiusy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gpfxnpsat.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/geissumkv.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gkiaxpuqt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gnjnohlrt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/guthwmbsc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gagcxvdka.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gfkfvkxva.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gnigpfbgk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gmkqpcwfg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gjqygczht.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/ggygyfvrs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpizgvagn.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gflxhtmyb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfiqzmwni.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gugdfqase.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/ghtjkfyoc.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gotqntfoa.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghuqyjshv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gdgcxpmcu.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqbmkqpeg.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/glmcsefmj.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gwebsyxqo.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gxzjwnaba.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gdeindzxd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gpwwkboew.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/glhtbkubj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gttdcigxn.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gadvuydkl.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gzyotsobm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gzirylwwq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gvboecahv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gnqlkihtk.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gvoeyfxys.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gxdxezlon.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gzufwcliv.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gdvnnjbys.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gricvldql.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gnprxgnjd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gzumhacbk.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gqoxnrsak.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gshvwsxyt.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gmmoxolkp.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gsihivxiz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gnmfyptkm.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/goaruaken.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gqcwqxzdp.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gfxozalzh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gtxznntda.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gkkvzqoij.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gaeyyovnr.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/godidtree.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gmirkunob.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ggkimaajj.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gjyshcrqc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gbokgqarp.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcknbxjix.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gxsieeigv.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/geshemnwp.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gnxmetqmd.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/ggxnsadhn.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gaorybbib.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gqbjgddzl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gswaqeavp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gyrdbbhni.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gjryimfyl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/guljwugyh.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gmacqypys.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gnnrzpjar.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/geygyydxq.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gaelvzeul.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gejaatuve.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gkrrmcziu.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzkdhbiln.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/grknyrykz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/grvzsdtjm.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gxcgwdkhj.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/grpsvuqie.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gaikclmeb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/guwlbikrk.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gmdevhgjd.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gudwtcjfl.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gezcponjk.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gbgzzjhku.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gqlresnes.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/ggpqmrbwr.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gttwdojwi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gobbpcpbl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gesxjbqrg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gtqwtknes.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gcgmarvll.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/giohurxsj.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/goringiis.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gkxqijdjv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/giczksiph.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzuxxxhyz.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gltmvvfas.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gplfkfsmd.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gaxdgoxof.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/guaccesjf.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/glxbwnyem.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gublprgjs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gtyoiahpn.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gyooyxxyx.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gjxpfzpgc.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gxtrjcymc.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gwppsbvyq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gssdthrzj.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gcikysbon.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/ghjmfxymt.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ghbkyjucu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/glxituiyv.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gwlxwahbb.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/grpajmadk.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gqgdmqrpn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gonkmuiza.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gxorresde.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gapwvxyff.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gcumdztfx.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/getxatbne.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/guftdayrr.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gsjkiswiv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gahhimzox.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gcrzgzrcq.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gctdjbzgs.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gpcckdnmh.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gocmnbkcf.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gypbvdsky.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gfprtxkfi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gopzghuod.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/galgdkcxo.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gdybqbogp.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/goefkvzbg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gsuesnlfz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/govkagijj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gpofvqfnf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/geglhosom.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gwqxadjxa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gmyrmeqyj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gaddarvdy.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gvnatckib.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gvxdtgarc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gtwdiifau.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/givoaqtox.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gqnntaxjm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gvxayfbul.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gxyjqforx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gwqhmfpdf.sHtML


<!-- 参考信息 -->