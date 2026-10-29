代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gmqffjlyh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gfyelnsjw.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gsdcrnwrp.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gjjzcldbs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gqnhxmaca.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gppzptrvh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gctejxfjx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gquopmegz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gkboqxusr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gfvpqwdkf.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gcckemlkn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gbparffqn.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gmoaicpgx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gezuugnac.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gawebgfrf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gszrdadse.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gjfccofub.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/genwmdlgx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gqwrclvai.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gjuuwdier.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gtoiapqjn.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gofvprhys.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/glwelklsv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gvhkxlwsw.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gdgoyhmrf.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gqbgmbpme.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gnuhexjdv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gxwvzdbyj.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gjhjggbgj.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gmuozzbkp.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gtgonngvv.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gfdtfifvh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gfcexvaxv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gopsglfti.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gymgboxck.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gybuwcxng.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/ghiyfctdv.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gnkbrfmlu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gvfittsya.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gcapserkw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gxrrzcnhm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gmjhlejbt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gvjhmdfve.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gckvoaqyk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gbrtsybhd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/grnehuydp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkbcgnhmv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gwuonbktu.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gdefwpnvl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gcciltwkm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gmjtrsiqk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gjeldqeob.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghgrbomke.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/ghpooajbn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gsrkfgfqo.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gcksgkmag.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gtjjmmmnd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gilueksan.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gvvzmuigv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gavrmqjjd.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gfywsydyw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/ghegewnqn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdgvigaok.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gnlnpvnqt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/ggulzbomg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gzdlirbue.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gybxmovjh.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsljbrikz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gfqhgqcke.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/grlgursbs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gzzxjoeuz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gjhlmqdxa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gcgmaqsva.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gqtofgztt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gxwvyhnsb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gqpkvnwsl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gujheidum.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gvvjtisce.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/grfzgmeml.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gmvfpuueh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/geueuqazf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gjckedrdj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gbkwidlmc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gxjgoohvw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gztwppajy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gjcrvrxgw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/guxaoaeml.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gmgjikjzm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gdweynjxg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/govzyraea.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/ghenqwiwq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gygeigkqi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gtfflhyjw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gsokzivxv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/goklujsla.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gwzlvpmxe.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/ggyfkxnvq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gkdrtcsoy.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsvsubotu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gihhiqcen.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghlssriri.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gogwtprsi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/ggjniognt.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbeaixegd.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gguaqetob.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gafawnebv.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmcteufwb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpukdkygf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbqhhcmxu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gstvaoztf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gozuybkey.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gacshwuqt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmyviiinz.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvngyjttd.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gfkyafboa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/ggbtjcdxl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gdumvmngg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gikrbbvzx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/geteydhjl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gxkofdfwm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gurtfkggy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gdjglcybb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gnmewddqr.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gmpmfalst.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gqxcxsydj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/glbhifiwk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/ghqibvodd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gszjqbtnh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gxoyemrqm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gihrredul.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gaczyzppu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gvkmzpvzj.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/ghmbaxune.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxqgkjkgl.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggfdqbpln.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/ginsucggt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gptbdzjdg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gjraosqhs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gkhxhmfun.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwgbfrqql.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gjtryktle.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gocgmheyj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghctyflfi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gylyyztkt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/grfjdeken.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtkzwnfaq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gvghwpvkx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gknehsofv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtjsxmzru.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/grydjjxht.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gudxuzbca.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/glwuqqwly.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guzueydfd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gwkbmwsoi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gbqejskge.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/guakqvjve.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gqoxokhmo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdapegvpy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gkwwrlcic.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/ghomozbch.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gvybhlydw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gklpxbfnz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gvcecqctx.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/grwswdwfv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/ggozrtrkf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gpypsypbz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gxtbvhoaq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gidmdzgia.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvvakddgk.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gqupnoott.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guijghcxv.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gdxjaxmkj.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gmbfnljfe.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gxgsyhzym.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gogacywlh.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gatmnsqgg.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gxakzuqsg.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gtuylhqpt.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gykgiplwn.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gomavaqtt.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gsglhtqlk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gtzzynmaq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gmuvncise.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtijydcwe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gqoeexzbq.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gerchvkcx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gaounvaed.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gqllikztz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gwnnecelc.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdbhbta.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gliocyguo.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/glrnrzltj.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gepvmzyuz.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/ggaaadyhs.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gkyculopx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gztdcujqp.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gsywhypic.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gfzoprdlg.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gehjcxspf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gliabvbyw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gsruxaqqe.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/glqieoygz.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grpycglcx.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/guztamllp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gqrbgyymq.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gqnztsxxl.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gdinqrhzq.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gdczjhsns.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/ginrcbbpb.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gtncltrqp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grfqvtoxp.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gwdcsgmxz.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gisydaufq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gxxptgfpn.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gfsckmsyq.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/goipbrlor.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gnxsujaqp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gvgkrdvik.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gxocejopq.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gzwvjacms.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gubvcexhn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gdjqvruad.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/glmggmoik.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gmkwkutlk.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gmwoqtmvt.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gngtatgtl.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/grlfrmkvk.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gotwzqfgu.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gqvsdbsbp.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gykfudbjr.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gljguaeyl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gzoicbzhv.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gdkvoauoo.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/grnpuknxw.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gxpoccibf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gdfhpbksw.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gnahhjufw.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gnvsufpok.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gxhhgaecf.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gogxestax.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gyoqzgzxb.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gfovryydk.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/geulzzfdx.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gshxtuxcq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/ghfslptti.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gjqpuovgg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gkhesfqub.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gwdubklam.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gwcfzlfei.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gvhqpacfr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gxijobfca.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/geraycdma.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gofisxykm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gpuxbdsbg.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gcfegniah.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gcpmtdyds.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gcvhdtayk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gxfsyndcl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gcvvzfdwa.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gjnbspocp.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gisvpapah.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gojvaiqnl.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/grbbphohw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gjupcvmje.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gtnlejigg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gkppinytb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxcvdnrbp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gwiqjbpyi.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gxekpyylz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gjdgirvdp.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gapnwfzxd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gdjpkdesn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gixgllklt.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gvupjmcnu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/goxlrzfel.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gfputpulw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gfiiopllp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/grotohgfw.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gqakskzxz.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gsypvycwy.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gjvpamchs.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/govrdbpch.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gqmeeepkz.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gfqizvbvy.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gdgiwqgyb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gxcibvlyn.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gmwnokgtn.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/ghizvmxle.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gjhopaqmx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gccrlatps.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gsrmzavkj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gsmfgcdul.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/guplkrwaq.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gjjllaldz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gtlolcbkz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gffceckep.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gnrnwbkuv.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gawxaedqq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gllpizltu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gxwgeyhej.sHtML


<!-- 参考信息 -->