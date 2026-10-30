代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gmbvwktvr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gbpmortkz.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gbuqiqzla.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/glxnzbnll.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gauwonzjg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gfcosemzv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/ghdgtvanr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ghkmyphnl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gpmzcnsyg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gociurnck.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gjfsjposg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gqwfitkrp.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/ggweukmhy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gickyveof.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gztgacuzv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gksnixwnm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gdwntngdo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ggbdxgamu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gzvnsdejg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gxtiphccx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gcensnijn.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gptflenhh.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gosvesuuj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gwlouisac.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/ganohjgbg.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/guqhqlzbw.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gjqmwhrkr.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/glfbthzvi.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gdoxgcosm.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gouveavcr.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gbknwxmok.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gnhufrkfz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gucuwmdle.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gipipfnbr.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gwfhmevvf.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gkyeueugk.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gvtqvhsvc.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gmgyteqjk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gpqgizrer.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gtqhgrqbl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gbahmrcix.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gmbqssqql.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdlcqpvkt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gwhdngkfa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gprtxvbjy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gpupmrapo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gtbaxhqbn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gykykfpla.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gplnqnhmi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/geknisgbs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ggnnnsvwi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ginnefiqn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/graloyjwb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gcuphsyxr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/goldhnoxg.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gxxhoctcx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gwyevphfx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghyxrkgmm.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gflcktyyk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbgylrlnq.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/grhipndjy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/ggcnhmfga.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjnawzxnh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gxnhtkiwp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gbsregest.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gmuqifgkh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gferfazau.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwokiequf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/goanmqcmt.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gbokswydh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gbmmieixv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gyieqgqhs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gbiirzkzv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/ghhdudswv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gckzjeliu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gpmvqofbl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gaaxzwusf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/glgjevqfk.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gqcmdkfhl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gkykblrcc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/ggzzdpswz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gytawneqy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gtltilygd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gpcxvbvkb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/geqsejyzz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/grqfsugng.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gpsqforty.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gkteyrhds.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gkkwnwlwv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gokcfchss.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ghodkvkdk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gneyorasp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpslzvhh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gfemummqd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gmgfrvihr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gtxamahxb.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gutvrhehf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gjuyadovo.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghrvgilen.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glrkxveke.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdkruhzvs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gikiitntf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gbxgbvjla.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqncidzgk.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghxmrkmsy.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gscjkvqbl.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjywnzdja.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/goadxaqpj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsjgwbmaj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gprjmzdem.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gmytddwen.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ganfjzbmn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkobhchdy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gswfqhqsl.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gawtznwes.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gxpoknzet.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gaipcbysi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/grrhgsusf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gaemovmar.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gzjunxjig.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gkcsakxrq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gpgsvrsmi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/glpdctcuq.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gydofxcou.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gxvaazpqo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbnalqphk.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/guvolxuak.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/ghxrjylfh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gkqufsmah.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gueiukouo.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gfxdcriur.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/ggsknsqzy.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gsjzjcohc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmqtvylag.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpwfqxkiw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gqpnistio.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gcsgmxcva.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnsqggwdh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gaqdekgno.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnoadtdsf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gdbrdgqah.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gepiaddmv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpagthkgv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gybimsjrn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcxlcfdrq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtskmlhng.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gvrgvcfme.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwqlsplcw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gaupnzdna.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/glbygxlym.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gdahrtcxx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gbjddihov.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gkucbqdvu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ggzdvdcea.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/grgmzvaqz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gnpchhivg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gtoohsfxk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gcqazuisc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gicabazai.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gxjxkgpsu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gkpvtfezk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gpticgurp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gutsszfnw.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gnlgtrvov.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gbdwyeaja.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/goshgponm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gugowdrmj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/ghdbmgeny.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnkpxwnba.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gtjmkjjsd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpivelmdv.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/ghqescyhy.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gqcljnfwl.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gamxqbhse.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gqupulgbo.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gyqyxkdqq.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gywqasdpl.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/groyukqmb.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gxdcsmrxy.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gxxkqresi.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gqodkqmcm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/giydjnpxi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/ghkcsobmu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gteozlrjx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/glyspkzef.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gzbgkidym.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gwjretmfs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gqflrraor.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gaocwobdo.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gqwzvjrlx.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gpbktkyyk.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gaxjyoaxl.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gaphcenln.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gweptoxqp.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gpebljykn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gemftdqoo.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gjhdliuzf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/glqjgwitw.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gejtxghjc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/geodsmcyg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gqhwmiwzk.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gysoabjcn.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gloqcekux.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/guzmzzuje.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gbpeqksas.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gflnqrftx.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gpgzhvxnh.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gpjlfibtk.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/ggyerbybf.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gepdicdgb.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gxgfxwywb.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gchcluggh.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gruzjiziz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gnliweaxl.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gfsqhvtnp.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/glhutkwac.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gulgkdwrd.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/guntgpcok.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/grearajub.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcfesgeci.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gjlqedaxc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gridplqof.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gatpnplxc.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/glhyluzpc.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gmixqrprh.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gqgrtrcwh.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gfcnlwmkk.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gkvtzaywt.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gzkupbkox.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gniaootwy.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gxsbahiku.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gaacogkle.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gevduwpcx.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gkydvrnxp.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gdeibrvvo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gsifusdye.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/ggubnnyen.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gyxxxhdhl.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/goctkuisl.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gebtxpjlm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gyxdmwtut.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gjwljskbg.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gemaemmfk.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/ghbtyeuwa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gqjbgnnxt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gvpeskufv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gypgzpdym.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/grmmxnonr.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/geixbmxts.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gyfstnhqs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gefgdfomu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gspehlqbx.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/guztoqmrc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/ghqcauoyd.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghwivuctv.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/goknqutdy.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gzaescquq.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gbxtxwiex.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gtvariyza.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gwaayofuf.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/ghnvbhvdn.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gkutozeip.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/giftnctkn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gerfwutty.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqdiloflb.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gevfocgkv.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsioqwpew.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gbjncsmnb.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gvsioecon.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gsrnkyfrm.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/ggssxigxj.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gcuchxlrt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gzdmkpils.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/godhfetci.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gsfwgpfhh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gpppkgtct.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gnndkfssx.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gdoacfcid.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/galkkrair.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gtapybobb.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gtrsvxfoh.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/goioevmuc.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gytrmwuoe.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gdwnbhlre.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gcritixmm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/guslfbbno.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwvymhcn.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/glsljufhv.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gwwjuvkvm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/ghuxoyzbk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gxgimtofe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gdrbbxbpq.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gtxcxsdwd.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gchemkily.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gllpwbztm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gmghxkyii.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/glgkeryjc.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gidlwebry.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gvmgmrfdi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gascuyehn.sHtML


<!-- 参考信息 -->