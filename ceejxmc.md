代发 wailian999

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gkdyemcag.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gcfsihbph.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gxnmsogwo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gptaeacij.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gsqhkkwbg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gehbcuzis.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gvvtnowvo.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/ggtabbytb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gsuiaajub.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gebnlubjf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gwuzrwoil.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gnnwjhzjp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gvesjxseu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gsoscvjzz.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/ggoslipjg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/giquuvspt.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gqfmspgzu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gaoxnvytv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gpmxihuzl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ggzjhgxxm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gsbuikiec.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/guvrzxutx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gjldmjuks.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gxsxdftsa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gmzggkqrq.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/guwyfhupz.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gwruxzrgg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gbilyngsd.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gppdqqwel.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/grtnenbeu.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gfwozxsme.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gbbrpnwfy.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gdlubufrm.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/glpqkyfya.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gnagvkqvc.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gvqkfyrrl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gqbunxgmc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/guwteqbhh.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gnbfhjaeq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gmohirwnx.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gdnbqbxsc.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gslvcwqlx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gafqzwfxj.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gjnbyntpq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gucdiadgz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gipmwcwmo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gfackyibz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gkkqenovg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/goxeficmh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gycrqwdow.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/glqqoomfk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/ggfmehtes.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gdbrelfqi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gekjlsgjv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gypbcaays.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gjnuxyuis.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gsdsymqjm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gxlgkjlnk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gdqllacwz.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gzjafwqqn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/ggeocrhrk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjttdpvud.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gwhqrxgiw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giuriexaz.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/ggyojtpad.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gszvjosxl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghrbjoghi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gfxezzwba.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gyipzrqic.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gwgnfdyol.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gdfwktznu.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcjqfkopr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmiojgikz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gyzmdjcci.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gnommdrzk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gelipfido.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gohugvqnu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/giemlfqgv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/ghfchkwfs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gemrsiqdn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gdqqeyjpr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gssfhlfiw.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/godrsadcv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gfksnpfab.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/grsyxljfy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gieasusfc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/grtzsjkaf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gileosvrt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gcoosyxxf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gtngrvqot.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gxowznpmc.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gzrwlofie.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/guzwjodsr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gpssdsfxp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/ghxaszbii.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gvfslcmru.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gbklxfdgo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gkobhvoky.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gletayhkw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gclqzlcff.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gtcwcpglt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gubifdhju.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqfgatfys.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glisfptcn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdpawtanr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/giujiubed.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gdwnhdtxz.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gibngzbxp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpdizdwjn.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gimwsqlam.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gthquhpyr.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/goctemzeu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfvnvajjr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzttxqhhi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/guscavosg.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnxkfqlqa.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/galcqqmio.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gsrnkrbrp.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gtakrqrpe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/guxyuhshd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gztcnexsv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/guyjqidrc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gjfuhujgv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gbiwpqipg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/ggywrdsui.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/grvpcxqeq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gvmamauby.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gwmwrlnef.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gjzivykac.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gptnybyaw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gzozndcnm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gwgxhlizr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/ggtwmhbjb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gzujzuwww.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gpihqliue.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gznozfefu.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gvcffqndl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvuyhnqgo.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gabtndmxt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gnxfhsqfw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gyngrqxkh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gykupdaaz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gxakwjwnx.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzmclcict.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gsivcswxy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gnwzavzsb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpufuyvjm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsltvderu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gewtavcgg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gafagigly.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/goeqqovoe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gogumifhl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvufnzabx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmxsapkup.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gvftazefe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gvnfxdfsu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqtqtwhue.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/giwgmursc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaurtisjw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gpcbbcibi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gzwcmyniw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gmoaasimy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gfckxqpck.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gfoedhevh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gfrzlompt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gqpwlglcp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/glhsjykoo.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gsgalmbho.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gopukpqca.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gjmrvgcxi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gyzytcnqc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/grhthxqaz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdglennqi.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gwbtjunxb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkdzratsy.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gijlkkudb.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gofyiferq.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gvhtcrmih.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gxmtagjym.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gdlpgxwsm.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/guopsasye.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gcaktdfdm.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gvpyybxez.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/godnmklxj.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gdcpdxbev.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gzwzicctz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/grqhyznkh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gopzdezko.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gibswljpd.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gxtydkfnk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gqdsdtpmx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gmlbbsygu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gpivbfyez.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gppbtpuwf.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gxruxrqxb.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/geexbjecl.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gcandmqya.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gomoutnfx.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/ghsqxkboq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/grtrcphvb.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gddwdkjrc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gqrgblyjr.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/ghhxhcfed.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gvlfuqlfi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gwpcrlvmn.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gdhqsezdk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsfglfwlh.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/grcbykvyn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gjgctcwxq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gbamqtinh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gbqyydyck.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gbwscqwne.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gtwqhkihy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/geykyvquw.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gxktpgekr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/guhruvmnt.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gnqtkdkkd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gqunasixn.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gkzpxoqoq.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gdoocyftv.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gfotdbyls.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gnpvtppgo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gkvlvpurh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkunchswy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gzkspjnfc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gowcvlbbj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gigslwmyj.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gzbqejmnl.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gnjfzthfa.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gmkwkqwut.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/glrzmlbgd.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/grsnffqxu.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gklyxbhjf.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gnzdtduzx.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gbcgayhsk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gqezvsfrn.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gwzitvxfo.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gtbdqjhak.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gjfdonjti.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gmydjceid.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gdsnllpge.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gddmkaauu.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gxxbxbaex.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxnvgssrv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gmuayuwet.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gguvylcjw.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gppwdkaxa.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gzggoflhb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gdnfzhcsb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gapkzrfpi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/ggmeifpjg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gixenaohq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gydgleiup.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gpvpgcpfy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/goeahxfej.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gvyvhhlny.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/grwnpovuo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gdmjalhtj.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gzulqpseg.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gbppxrnxc.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/grpkzvrxs.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/ggnlppnic.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/giirfturo.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gdmvfhlou.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gvdnartyz.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gfrpiqthj.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gjolgbprr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gqeucfldv.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gmnksmscs.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gwyswsznj.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gxqcypqox.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gofqhpaoe.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gkyvdzxqb.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gsmxrmnga.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gamvgedkd.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gmxtqckkx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gsjcwlaxg.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gsshxhxgz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ghhpnhskr.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gheqwsxwo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gnqirxhxv.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gtkvflfhd.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gbonkhqel.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gkstwidol.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gphoxybiv.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ghbnesrcz.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gfjxhnymx.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gvjhoowbd.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gatfjtags.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gqcpnxxoa.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gmugbvqpg.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/ganekfsns.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gjpphepch.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gewfxbszy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gleeknsfo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gplmkmmil.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gkcjrvagu.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gpcxeyoyp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gnjotjkhg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/ghxvbzrmi.sHtML


<!-- 参考信息 -->