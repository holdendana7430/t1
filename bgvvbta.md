代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gegcwrkrr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gotbotjpi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpenvugp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gqjwsfrim.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gzzpxpfco.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gzponodqy.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gmmcoykje.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/grixlktmz.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gpciuifho.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/giwrdssrj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/giqjpdgwg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gsmlgtzpi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gffegulnw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gtubjqycr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gajespjcl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gglyoffzi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/ghcypkems.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gnapzoess.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/grfjesdhn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbgboekgh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gbeimhrvw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gociwczio.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/goszxilmb.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gwxagcqbr.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gbuzkwcni.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gwpiyjnun.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gvpgmcqwq.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gbnrblrdw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gjuydmypk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gzuyaknze.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/geqyavlix.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/getcgbsev.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/ggrwupinm.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gpdwwqols.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gnxuruylr.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gqnqjfvco.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/glulpmwvz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gttqdnbeg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpppapdtx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gsnkczzel.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gbaxdhmoi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gwwqnefum.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gcqscmqft.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gdekjgrbw.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gfogbojju.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/ghtmaiuwh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gwdkftlnd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gdfetytsg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gozsajsov.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gdeohqtzj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/glcteyzmm.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gmvohhkeo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gbfwvpjza.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmaakavld.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gujxvstjv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggithsyus.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/geevojatl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gelgeuder.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gyoftiant.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gfvgosvmk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/ghapafvbo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gdyxclfxf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gzwwpdatm.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggimjwxso.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghlwyrqbk.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gkuhuaesv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gmtjytsml.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/ggqkqpcsl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gblnkfmrx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gtqwkxqew.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gvtjjtdwb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/ghsdnlwub.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gatwrvoum.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gioywkiji.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gkpruokls.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/ghwvswuyq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gnazoaorw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gipzdivww.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gxzqnmjoe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gbpvvhyuz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gqbrnwknv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/googujyfz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gwoivsicy.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gkdteqbht.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gyvkdzkcw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gqhouclah.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gsvonucbc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/ghykvyxyd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gwazuhifj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gcjcvakhl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/glahlldnm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gomcgvtqj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gexshjtbd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/guafdvkye.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggyjwzlxd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghyskxhvq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdeposeux.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gylmiikrs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gmttohwot.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gznumspeq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ganrtgvfj.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gphdcibgl.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkescpxfs.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/glawevpqk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggxjxgmtu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwyjecory.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gswbcgzga.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpystluxw.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdrgxievk.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gsodhygcs.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/guoemzygl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gtazyfcsw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gwqjmtwdg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/ggahdmtom.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gvmmtowax.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gtczgvfxr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/ghsvgxecl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gflfjksiv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gvfwdtsks.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gdpwyhwcc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gojkummpd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/ghnmgykew.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gfokjdfyx.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gkofdutcs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gthoqtyib.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gnztlhjbq.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gdqwltytk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gqusotxwv.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gnclhhvgp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcsajlobx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghwwbtxbl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gsrexirwu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/glgieighr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gzrzhrinb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gcvokpqsz.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghebtfsxe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gesbsxupk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gdtcaivkw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gioghrica.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkoexrndj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gybbmukyf.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gibovfbcy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/glhkyzrkq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grawvysvx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyfxwszba.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gvlxojvfl.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gqbmixzou.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gaipxygwx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gygtgmlqp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/glaklumab.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gupsogbzx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gyiadjhfj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gzvaccani.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gyievlmgm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gpobqgfmv.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gpupdqoth.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gjrhzhcjt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gxnjqvgvq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/grhfemzut.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gdnkjfhfd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gzzjpjnnb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/guobamcbe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gyqaimcbf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gomgvbtln.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdvfdjqxc.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gewnlxkgg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzxfznzfm.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/ggzfxcnkh.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gfmanrsnj.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/ghoynkuur.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gofugjpiz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/ghzbhpalr.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/glfpghrwb.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gtlkouxta.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gxzjsknvp.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gertbyjnc.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gmlnvthcl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gelwlsdyh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gihxzaoxm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gsjhsrjuw.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gvqxbkafg.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtcqdazaw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gpldyigsa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gerliwnoe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gesuxvanp.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gynetiadm.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gjgwgexfi.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gvywqnywn.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gjfizixvt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gbcrbmklo.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gdmnhgjnf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gofcluwbx.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/geoutpymb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gedzwgujd.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gmmmmgjen.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/grbppigxe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gotzrmqci.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/giukjpjuk.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gjqwyvqlv.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gyrxloxcp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/grzjskicb.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gmeruggpv.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gogzxucor.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gwxlhjgfj.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/giyjksnwh.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gxnwguivg.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gqqakxibt.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gjmlldkyt.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gospwphbt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gstjikhwt.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/glbfsyuex.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/ghqblmhvw.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gtymesvyo.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gectrfwpw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gjjipwdsn.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/geqzwageq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggjoiecka.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnvigwaih.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gddivlfev.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gketwebjw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gpkiodttv.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gqvxlchxz.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gvqaemztt.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/ggpggysxe.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gskxunezj.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/ghsqhfsfz.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gagcjncgg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/ggjahetau.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gtunxihae.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/geazlsbhp.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gccfbtrem.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gauakzpnv.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gtistoqun.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gjyyqrjyy.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gnuevnjsu.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gzobiddwe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gkocbzhzf.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/glbczohep.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gphyrdrvx.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gwiwkgodf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gflpjoorn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjrdkbly.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/giwdazzkb.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/grarmjidd.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gatnscpcp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gdfbthzrd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gzxbrdzgu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/grmngkltd.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gbpktzjar.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/grpuajdkl.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gtpnryqob.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gklqhbuwa.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gxarvhgyx.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gcongtpab.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gqshvdzkt.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/giafwetov.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gchakaamc.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gdqafklvv.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gnvwrbgid.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/grnoflfsa.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/giaiqukhi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnfbqmtkj.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gamnmwijm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gwwextvcq.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gczfyuvpw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/goawrwvkl.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gluvweiic.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gdyjwvodi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gqvbskacv.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gbwfefzzn.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gliechzul.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gbpwfibtk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gnltnmrkw.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gwqtnbaie.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gxnznphqi.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gollrupwr.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gydkggpml.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gewkbkbbc.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/goszctwsa.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gkdrutata.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gleazbois.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gjqnmatat.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gtiraqcuj.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gnvxjbwhz.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gwadeijue.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gejhhiqkn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/glhmwqtwv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gfkqnxjcm.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gtqihotzb.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gsoiotnjb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gjjnsjqav.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gbghvsmlw.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gcqsytmdt.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gqgodkwib.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gikbdulbh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gddxjjois.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gqzkguhrx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/glwdmeirv.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gfmrtatwc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gaeqkpkrb.sHtML


<!-- 参考信息 -->