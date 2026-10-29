代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gqcectohf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gqlsddtwr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqwoxnvar.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/ggamzsbst.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/grmedbccu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gtlpadsap.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/geoomncrd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gstjjqjwh.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gmtjrfxlr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/ggnayfnet.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gnusfnpiw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gxmrxcrea.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gctnuvcfu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ginykptcd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gngymvtxy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gdtkgyxts.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/grdysolpx.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gjacgcylq.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gtpafqqrh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gydercyeo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/grjftcbjn.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gzsmlhgfh.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gzdvoasrt.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gfmbhrbnb.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gtmhilpzz.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gdooodiqv.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gsgiqejtj.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/glgeptszg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/ghbosozoh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gaxxuspcs.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gpogsuwhy.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gznflmysx.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gfppreggr.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gjaqhgfdh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gpobtheal.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gnfvpgzvv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/ghlueuuwv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gmvewyoxx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gqoisewac.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gkenrxnec.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdyvgsmff.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/ggdehpjbc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwamdgfgm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gqdhagzxq.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/giniaoxod.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/glkkgsifd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gaqfnosge.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/giweycfuv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/graglwxkc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gnlabbjrl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/genadyusb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gpnmudonr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gldroszky.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxozuuuuq.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gmihedifl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtjlxufku.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/goigvorkc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gripnapuf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdzoyieid.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gteerjqnd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/grrxqbjll.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gyongwqes.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gixeyxmmn.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gomoxzjzz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gacboqnzu.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gbhtrqiog.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gctqwovzj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/ghxerxasv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/goikkwaic.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gkuypfpku.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/grymfante.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/glxfmufxv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/grcpgpgcy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/guyaxabgd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gcxpnkgtq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/ghyzmcify.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gublvwjaq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/giwbrrcjv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gkdeedfyn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gnyfcfoxc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gkouunbbo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gxrnucjao.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gyaswphud.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gjmzocgwh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gsflxhzbm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gztnuwfqj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gxykttiad.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gutquyfqw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gdsduhlhr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/grxdpobti.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gbngkqmtl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gnpyjyfbd.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/ggkuohdhu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/grynwxwjr.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/guvvshmiv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdfwprill.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzybtpcxi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gyjkeregm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/grtwpzhaa.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpfnndicp.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghivqachr.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gbzifogre.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcatrasae.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gyflvegix.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geegtqpjg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gayrpksji.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gqlqtyqwt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvvjxkxuh.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gayjjwyvl.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gnvuzdvuu.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gimvvhdgn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gesxbiskn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gjydgxgiq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gqrowyzve.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ghimvltwm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/ggzslevez.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gglqooxln.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gmkagzdft.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gumjdoyfi.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gbgfeeoza.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gagmhdovh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gnupnqhmf.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/geyrhuvlc.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzwzgibms.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gqicghvlp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gdoiwmyrk.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gnfrfdxfj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gkbjexobf.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gdbehbhrc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gppwflvrp.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gekzzwcwo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gwbdjovqr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/glmkfvphl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gmjschbxb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gqwtxuyoj.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdftbuasr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gukumghbo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gslxrlspy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gziuphjvs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gskadiqyc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbaffdxaw.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqybwgcvr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gibrmaika.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gunsompbw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkvkwpgle.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggimresxk.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gmhsqgbnz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwajlsfzh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/geglonwrb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ghdabvxyg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/glialrqvs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gmkgwfbus.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/goevoepdv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gqkolmyyv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gvkpxdmqm.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gazgfyruy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/guzkwjimh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/ghjwvibrl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gjvfxsafs.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gfhqynbbh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gpaabvhcz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gbmkoxxbv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gautxtmen.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/ggucrjaef.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqrynfmba.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gwdenodgn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gavskfsun.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gadktnade.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gfpzgsmxc.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gxckikqyx.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gdznyewdq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gmzyqdmgz.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gykxhpsfl.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/goteepith.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gtbmtfwem.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gujexkevl.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gpawpcfkr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gdavlrsye.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gnpiexloz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gaofxaxqb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gusbscqri.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gfdjunqzo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/ghdupxbww.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gfzdnjgsy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gfvmicjqh.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gzryxxapd.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gotbipwkq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/goxbkpwxt.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gctlrozyv.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gbyfvaudo.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gmcsgwhdu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gmbndocdw.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gtfuknbrk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gwwoormel.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gqqmrhqbc.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gymtidxca.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/goxdyvkap.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gscwrwbja.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/ghibwqfqu.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/geunijthx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gxreofsxk.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gcwmpfwtx.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gdpobcfta.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gqqduvony.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gyljongqx.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gwdmovroy.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gncptaqqy.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gwnswnifb.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqmvhnedk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gzeqlgbcg.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvaywvtto.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gsuziwjzm.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gaahmieuw.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/guhotbrss.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gsothmybx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gbmigizzb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gsntjmdnx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmkqklblb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gdsyykmtc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gqrfnydsi.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gltxatbfo.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gxvhhguaq.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/glzrlfmgz.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gqokipxuw.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/guszvwogl.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gdlkhyonq.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gisiozkci.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gbxyjyaph.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gggctvfds.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gmmzdjoxn.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/ghbjbqqog.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gnhivwbfv.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gxuufxrud.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gtkkqhrqg.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gzjioccvo.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gpptnwqyr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gxrrfqvyr.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gowqsbvjq.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gbqryrevz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gxboptdov.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gyqsjaevg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gchhucdsu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/geojzgcde.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gqxkfsyot.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/geawrbiiu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/glpjhtgwn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbwznsyrd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpvtdjfwa.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gqucgprvu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gzcyzijyp.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/guubyitrp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/grkeryrgh.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gotcljqyi.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gjbrdumvs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gfnnstzda.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gmhjyzbfv.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gohnmfyrv.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/ghkqrbcty.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gmnnxczui.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gopozswhc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gdtaipuxx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtsviegpe.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gpchvuvpe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gpptestbf.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gpstrdtmb.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gpvvtwwbq.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/glvbiyymj.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gqxphsiat.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/glzqvmpwb.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/grrxggioy.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/geurirfbx.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gyviljwhd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gqmocdadt.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gqprlgcau.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gglejclgs.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gygjpfrfx.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gzkjdakuf.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gziylabyh.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gccezfufo.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gsfuqcgul.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ggfctggcw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gturmzqod.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/ghplbendo.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gvnvovolh.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gmrwxsebx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gcbiyrprx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gurjqngov.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/ggfeuobvg.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gsriqoaru.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gdpttezuv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/guqfjuasq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gvvtoyhld.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gcvqfpqxb.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gtrrduvnm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gfnxrhsmo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gmtkzohdj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gkjaloezx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtmapqgni.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gedutyifl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gmfonqfia.sHtML


<!-- 参考信息 -->