代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gdcprxdvj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/goaipqizq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gpgplcnrv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gpqaizyqi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gaupwdpje.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gfjzcmmaf.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gzsflhsop.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/glnhqjcbe.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/ghubqwuts.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gfefgkibe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gqdxdjxtu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gbtcqrlzy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gtajcihes.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/grksolfvo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gbiwnfxmh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gyddurmvs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gpcdshtwx.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gfkdqwrvv.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gnxmadexz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gcykvizhn.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gqioovhfm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gcgqqqcyd.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gqfhmhgwb.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gpturotah.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gznjzgoii.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gwwnmavfj.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gqmpacbbw.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gcvgsoolu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/goqrkhzuq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/ghospzote.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gkzzmwnyl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gboswhzye.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gxshquifa.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gqigcoisl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gvazidrla.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gqxrkostg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/guahwxema.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gnuoddnqj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gequhzsez.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ghsnifwwh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gqaobpbnr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gsdknyfby.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/godzcheqj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gkhszfpvn.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gkehupcom.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gupdvdguk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gwhokezir.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gbcnoebhl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/grndxratg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gdcmnujuq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/glcflogda.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gujllpwgq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gisvcozhi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gidgxppuv.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gaufkctlc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gabajmwwo.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gbfycfexe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/ggspxjxqx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gaicguwxr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gfxrfoblp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gifzcgynr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gsaaovnle.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gmnncfvdj.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfqkddtoh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gnjcutole.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/ghcghdrgc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gwaslewsi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gscaxwfkv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gjheozowq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gwmfjokim.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gsjoakley.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/geoyjydjc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/glkkeffko.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gkzdfncba.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gkrdetcfn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gbzxlapfw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gvoauxbfv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gmjdqapmd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/glwnubuay.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/ghuejvjof.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gljotvdhn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gwhjgcdmv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gqgjtxxay.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gfslbdmaq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gioagunyq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/goszhcufh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjjqfnnvg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gbweqpnww.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gbpbzmdpx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gsgwalfpx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gafxgygbn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gintaiolc.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gbrdvnibt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/guvmhrywd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gymfcayap.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grxqulaqq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwgpblpwh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gtogpqdsp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gedpvirel.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcyfgifwq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwsevhuvb.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gxvgrfqov.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxsczhxkv.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gilsrmvny.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzgrffpqi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtblrifpm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gfcxajsgw.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gklwigpus.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/goeplchpo.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtldcmsbl.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/grtcenjck.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmkgybaas.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/glvvvitin.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gnltoblml.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gzqaiaryq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/ggxtfebdh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gvwrtrdob.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gztezrbon.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gbgizlztd.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/ghuarydrv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gackknrpl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gdumqmrsi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gdehsogbi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gejtxlgfi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/glyygcinw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gwcwparlb.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gymyqhaok.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gizyktkxa.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gixovcipt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnmdqqvbd.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gurgvnvqz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gldwexrfs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gudvxjzcf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/glbsjkqst.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gsrwqedet.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyqpdzupm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/grxvxmmdx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/ghbmuavzz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gguhzpjsf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/grhwertrf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvnlgrefs.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvsftlycq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gsplhotsv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goirfwotx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gbgsqkaeg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gvldibucg.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gqntkpfgx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfmyemtng.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gkhkzmynr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/glpfyffbt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnnchnabz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gjnrsgqdh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gmcdioxbc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gfeixvwmk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gpjbweqpe.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/grhltrszs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/grjtprfqc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gpbhwivrs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gbhaeqrmu.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gzvpmdaqz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gfsmtbuqz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gqzjbllkf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gmxcliqtg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gndtabrrf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqmkldkri.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gvoyzduzs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqbbfcgef.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gvnvooidn.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gruwpghrb.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gbvbcfizg.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbqhaiorm.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/glirbgqpd.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/ghpotiszj.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/ggusokmoe.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/ghzwpzxiw.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpofkezxs.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gxoazmxga.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gmfikgqog.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/ggthcpims.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnihivbzf.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gnmnsttdu.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gzkvjkcyw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gyartsftm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gewkgvizy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxiqugydi.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gvpvrknkc.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gzpgwpdwx.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/ggvgbvgnk.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gjytvftky.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/ghowycuhz.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gotbacgrt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gmdlrtdie.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gkefnarwh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gfktgbanf.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/glwdrndwc.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gxebhyvto.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gdkmqkiqf.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gwqelmdbk.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/giebzgzzl.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gmbfdotim.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gkhtkuprg.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gbgvloxng.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/ghnvzyutd.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/ggwcustqk.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gqhjfvjcp.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxjxzvjov.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmvmugskh.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gechfshxf.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gxsrvwnha.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gdtmuuhtl.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gfpzegjem.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gckpewzqv.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gusdrddaw.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gqtysqukz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/glfraoiju.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gcsprcndm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gdjdazcln.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gkiiyccua.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gfxbowbeg.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gkhmzcmrb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gzncyuqyg.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gojwjyxup.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gcdztbgvj.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/geltadbet.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gmjcdutax.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/glnsesgmv.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gfcizqqgc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/ggvtognvk.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gekdnnzci.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gxsiobhwr.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gtoepzaxz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gjcuohzum.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gpclqelwa.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gbgfwazuv.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gkssqfgcf.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gxqynxvgz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/ggqnnrgys.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/grfkmsula.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gnsfqipcn.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gyjuxbetx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gsbaarlrd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gxooskngg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gbtxxzmqm.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gufnxoynr.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvuegwwpq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gslanpdbp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gcwqycvbi.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gzczwpvdt.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gruaduftz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/ghaggcpcr.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gwgdghydl.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gjeaghqve.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gltbkwlzf.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gcuxfsoew.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gchxklcfh.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gbrdgjxme.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gngxwmnpf.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gjjpbnqyg.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gsucdsymj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gcdyhmnqr.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gwyfppybh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkahakpcb.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/goaqpnwle.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/guhnrjgos.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gaongurtl.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/ggplufqmq.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbnaksmmb.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gyxbatexe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsaodrtxp.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfnvybttg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gzwpiouim.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gjmnlcmpy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gvjajemjo.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gevdjgswa.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gkdygqowk.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gixqugbuu.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gsflhogod.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/giolcddyl.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gjidvsrul.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/giaqkmvnt.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gtminrhcg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gfzuiojvg.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gaqrygdsn.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gboyrenqa.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gnuqgsbyl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gdmangntl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gedpglpkg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gkkmywblm.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gnncqxtqn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gxgngekkl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gfgvqcblc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gbdpioerb.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gvohilvce.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gjmsbkqzd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gefkzkfob.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gssvccikc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/ggbiamxqr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gkgvpcrav.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/ghvdtqhfe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gmmdvnpir.sHtML


<!-- 参考信息 -->