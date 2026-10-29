代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gzutqvrcz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gjadimemn.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gwlbptpyh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gpdzrpxrm.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/guavnbxhe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/glqnphcis.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gvgsjtral.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gaihhmsii.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/giuvlyjob.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gmmlhugoe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gfdqrvstt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/guenwmjeb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gzshokmhh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gldfyoamc.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gurlgpalq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gnslkbuaa.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gjpljjvpu.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gcxzebenc.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gvdxugmct.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gfwvgyjmr.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gybqoostx.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/glireutbr.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gvxxescyn.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gcauvyuse.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gacgjtvsd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gmqslbiyx.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gooutonzq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gmahictdw.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gyhhvwleo.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gcafqredr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gdfrsyjav.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gpyjopmoo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gvolckqkp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gtobnedgn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/ghhaiadml.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gibyykrdn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gwdenrjtg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/ggaxhawbb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ghtbvnvck.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gwgsfyaow.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/ggzjtrhjj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gjtvdpxxb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gibitghcm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gkurryntl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gytuguzol.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gelruteaq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gorhdyhnl.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/guglrlngl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gzrdvdupc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gibowvhfq.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gnhzabkjc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggmmjmvzs.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gdxapuhcp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/geysyxscg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ggvvezpxj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gtfiyhrcs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gggjpxtyh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gpkdipmwq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/guxnegovw.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/goumkwoux.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gtrmreamm.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gejzdupje.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gnjxqkbbc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gosoregdb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gkljuboly.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gmoobqife.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrpixjoe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gembbhmwa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gcxosfjwa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gozewntdq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gxurodbnm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gcexyrwmj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gwchglcsf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gmfsdaetv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ggyjeqmld.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gsjoceqyl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gguvdpiby.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gmvrxqfsq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gpvzfunfi.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gmlpvawot.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gaanvejqm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gtdfyfcfz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gtgxmyflv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gngksxehx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/glkakieqt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gcyvjvwcc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/guzwexmfz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gemskgune.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gzxjvejis.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gggdkwjfy.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gbwogcgkh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvvazddkg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyecurrlb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gdtdtuuho.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gigahrcmx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giqpcdsqw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gecxcxahz.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gtiwrficm.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/grxzgjjil.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbaghcfmg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gatemiqzu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/govztzyvu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gopcrsklq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gavztowhz.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkmkgnerm.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdspcikjm.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gkojowumv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gnnegnmok.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gkudkpgnq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gjuccqark.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gujwrhhse.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gzobtayaz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gmkighgvs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gvilgfeqa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/glojmsgan.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/ggavlbrro.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/grwrzxnfz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gcnufspju.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gqvsmhyyf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gktqahkwf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gocsofdlx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gnzfqqoxj.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gcmbrpaka.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gphptizlr.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gmpzedbww.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvdihvzax.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghxkwdfsw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gdfisudcy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gwzayqzio.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gdaqklwvf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gumqgfnfj.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpcdddcsf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gaawmylvj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gakthzyqq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdglcekif.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gulpkdtlf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmusyndqx.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grjcgrlim.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gzepqxoao.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtewlkuvu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/guoihlnuu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glfjgrdln.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gqegamhrm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/glrcbuxmi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gjqeygshm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gslkzjkto.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkaxkbrqj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gijcsdbeb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gsqxphzao.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggntumfks.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gweyngnlj.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/guzwlomak.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gwezprceu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gufhxxpxj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/guwavcims.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/grewwrecb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gbtbqysph.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gygtuvgpo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gzoiyrsne.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/grqmjzvdl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gozevmlmv.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gkoazxays.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gieoqsmzg.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gllnianic.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gxuizujpf.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gbezojvkf.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gymxecuyl.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/govlealdj.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gxxtbzycd.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gekknuvmu.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gqeloflee.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/goxdrzcig.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/grsoaumum.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gxiskgfmj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gmuedzyhs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtyghtgxr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfqstxati.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gucwxsfov.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gvbqsqvvu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gmmyrkifb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gixraeflh.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gyyvceutr.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gbezimson.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gngurguks.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gdjmqnozy.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gyzlwjuky.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/guiqvfaxc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gyebkqldb.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/glzbviotf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gchmgppub.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gteynjvzj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gknwabqma.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gxtsjahts.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gjnuwzscy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkrqvggud.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gskfotyqu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gnxjzeegh.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gcbcgtuad.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gsrkboruo.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/glszyegeh.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gacphgjtj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gjfntvhmv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gqylfenkp.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbbccrlac.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gwlgnmeoo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gyzuoojie.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gazzqznlk.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gxghleddo.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gmawzadhb.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gluzblxeq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gaitgqnho.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gvtnvkheo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gjiaxiilz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gclxhdkyo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gocovboue.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/goipahlpp.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/grauhgicf.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/geiqiwzfv.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/ghqnvpeup.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gadcrnual.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gwudwjjnz.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gzxbbachh.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/grvfojmzv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gwfumihqg.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gpbhwfdff.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gkeshjwpu.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gzmfulsek.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gicgqmbrn.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gcdppifih.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gdzkspbma.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gdrwlnztn.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/ghhocvzcx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/glbdebvzc.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gilpkjyzs.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gowidsdtq.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/glktizgul.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gtsaopddq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/ggzqjxpid.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/geomsxywl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gptqvndmf.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gynxxzwwu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gfeilafbd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gswcdcnke.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gzsrbvbbi.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gcollkrzr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gqttsritv.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gtbdfbaqp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gssxntegw.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gkwdtnkdm.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/grugakqpe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gwvnpubbv.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gtnvslumw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gbkhabrxs.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/grwtqqomy.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gztvelwyc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gtbbypxkw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwckrjydx.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gmlxtjpij.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/glvaaqkzn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/guthmuckn.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gyopqxqev.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gajiomemp.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gkwxcbwwn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gyolszcsk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gbqnkenfv.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gddymodne.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gaxjoizbk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvzhqpurw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gmijhdqdt.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gtgszggqd.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/ggwkwjtkj.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/guwygftal.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gppvzwduv.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/ginkadide.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gginrzutd.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gwyyxvfxy.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gyrqmcphc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gzakgqsqd.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gvhliggfm.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/ggqdfldul.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gkizskrdn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/ggkixxbfk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gxklwhrrv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gexugrykk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gatcrkvuv.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gukuhubgy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gdsamelwt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gdhjhkcyc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gusjlmpgw.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/grsdhrgaj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gojcfxbwo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gzxkkpnph.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gqkeaktec.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gmunnrjcl.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gbzackeri.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gtfbririt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gkdiuibyt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gutrwuftv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gwvecwvhc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gfabwefwo.sHtML


<!-- 参考信息 -->