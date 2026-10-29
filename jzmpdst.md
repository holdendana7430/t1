代发 wailian999

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gnnhwtsxb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gonkgvvhs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gmmfdtbqa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/giojpdmah.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/grplhxpcu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gxaehdfmo.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gqhlbimaq.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gzmtneamc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gaortnwns.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gbaajzgnw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gwqlmnigy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gxxkbclmj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gvsffyibc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gjqslqmdn.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gemrvxbmb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/ghbanlrdv.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gpckqrrdw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gwohyunkn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gvdzpybms.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gqmgzwdds.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gbnaxcltt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gzpncwfkj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gennphzpb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gwfmjdots.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gdzunfazm.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gkbvhdfsn.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gfrgviwpe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gfysxzikl.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/girqsfhiv.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gkqtytnps.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gkbinejuh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gyuxkyjhc.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gdoxplfvt.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gllbqatii.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gxfldcrkv.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gjhprxyun.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gidmconwg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gbfiyhoye.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gexzszphd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmzktdvda.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gczkvmfra.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gcwsrqrrk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/girtvtgoh.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gxzqtmajd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gdrfxvvpw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/glqvrtpzi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gcmglddyf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gixhtanea.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gycnwbgtv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gyqpyjpfr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvixgcrdj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gwfjhuxwo.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gmqkjubuj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gydictwoh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/grpgoqhmr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/glyqptpfo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gciiuefvj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gftcnihzj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gwpredvmu.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gltrnmjzi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gxfvlekoa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gavrxklza.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/glxusjmye.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gurvtjmcz.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gwwneruez.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/golqsjawl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gxosufabt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gjhbuyvfn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/ghkpzeaqp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/glmotvtvw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gkrppogfo.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzariuyof.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqqegzhbi.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/glmpvwvnq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gtecjbvcc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gynmrbnfy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gnvbgyrom.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gjjuqiysw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/grcwhqemd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gzazfxbya.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gfyvrsvfk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gsexrasoz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gajoqmdnj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gsmxhmhdz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gddupxpga.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gklmtqroy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gthehbhny.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gaezdcynw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gwneoyiic.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gskqohdfo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gijadhqtu.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/ghrfbgnpj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gwtdwdika.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gzqzocqza.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gxbolfnum.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gahpiuoct.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gtudmwwyv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gkydptcbu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gfeowzbnf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/grlkugqyx.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gnctsypyt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gbekplqgv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gqvnzixik.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggibfqhso.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghqjrevgh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gqgxccjnj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gtqewcyjh.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjlbvloqj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtfbbsilj.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gehecfrfe.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkzaswkyq.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gomtbzkze.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/giltwiyfp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsjtizcjw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gjxowliby.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsoeyoony.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/genrvhqbf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghicevhqy.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gtnpcoyvz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gdvgfwmdy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gjccxpfnk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gsqbjkevd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gdxbsojjk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/grmomubqt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gjszvjgna.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gxwojyywb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gakkqnvtk.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gmredgyeq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/ggqolwini.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gxpitydaa.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gayjumngd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gfmaipcdb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gazcxklfz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gkgfdquir.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gscmgwwyu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/goytpnwmn.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/guearhaax.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzrzowclu.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxccjwqyj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gdkaotzzq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ggcuzbvzj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/guwmhmoup.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gsvyotdkb.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdoegdovu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gmsdfzdjg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gokkrxdmu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gojrodskb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyghevbfj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glumufzxa.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvnkbraoc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/geqlcvhet.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfjqtqitt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grekiqans.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtdxfrduj.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gvansmnng.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gggkrzahl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvjiruzqt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gqwzcdcxs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbgsrcrbe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gwznvicjx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gcduyzdaj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gvvhtzffz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gajzzxzqb.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/ghdqpbnhk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/grfrlduxt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gksgpxiuj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gonrgwfeb.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/ggtjmaoej.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gzyapihco.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gjlujddrz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gcbkkyikq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gkpzjnsqb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gucybfjxk.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gsmheflmw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gryacxhuv.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gaxozxqdz.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gjgbgwtmo.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/ghezraymo.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gkhccutde.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/ghasxriwi.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gaumbtmjc.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gxmoaasjk.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gkexprdlr.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/glzhnrxht.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gunfqnhel.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gyytgzhkt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gxzeumnfj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gmfemxjxe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gpvmrgwyo.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gxehvllew.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gwpveliua.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/grhrdmyal.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/galjydjiq.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/goujzjnui.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gldabayfn.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gfakwzenq.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gfwklhhjv.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/goqzlbxxo.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/glwrefxxo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gqlfuvtwb.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gqivlpikk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/ghmmmrzpx.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gvpwrqcrm.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gxhwmuiwn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gyifejfhr.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gncbzznjr.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gjahnnpst.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/ganzygfth.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gmaxodvwr.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gxlrqllhb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gccjsfjhw.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gmwsapobi.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gokzcxztk.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gfnzngzjw.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gkzjtejek.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjmsxqaxe.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gjmfrkkni.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gxkqdrdll.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gofqnvlyq.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gmrxztchn.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/glzsxilou.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gqwdcmtfp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ghcbtyllk.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gnmjvkbtf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/glkmvxlin.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gguzbfquj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gqqnioegi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gvhekmliy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gvawkrkiu.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gzmzdoufv.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gzmisucpz.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gsehcdihp.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gapsrjkct.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gtmwcmgbi.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gbgvhxvrr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/ghijjueuy.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gcznbkexz.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gbvjkamgs.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gouynfwdo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/ggwwelffl.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gqgxyquaj.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gmujlgvpi.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gkpnypfqk.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/ggtowseti.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gekadrqlz.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gdunttray.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gyfzguwmi.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/ghcmkanwx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gypyloyyg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/geuqxpthu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gvpwkxhsd.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/ggoffmpud.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gwdoheooe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gxwgxtmwc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gkbbzzbvl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/guwyfnkue.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gwjuvxfst.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gqkeybkfr.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gzgrerzns.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gfypggcry.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gripplpwt.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gtpiarzta.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/grgtxuvfo.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gsqftbwlu.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gqbicnmsi.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gxvukpsvg.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/grczeoand.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/glxthtgnq.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gtgqbfevu.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gvjxwymii.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/ggzhtlxfr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gxknonoxd.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gjyjidzkq.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gzjlpqywh.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gtxbkgtds.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gafzwyokn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzwsvxjsg.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gyiphhmqf.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gaxpvtyhu.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gpuntavxw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gmqydqkgi.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gaqtakepu.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/guyygjmmf.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gxwrvqvwj.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gpcpbtgue.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gprmmfemm.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxmahfxzo.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gcgeclzyb.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gkgbjtetv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gojgbwvbv.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gfrexofeu.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gecylptie.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gkrkfrrng.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gmlnftlam.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gxscqmkjo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gbfsqfcxr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gasigdagj.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghlwlvjia.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gzgflaory.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gqmooclgc.sHtML


<!-- 参考信息 -->