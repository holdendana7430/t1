代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gvzhrgzwh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gmeeydlqm.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gqtjdilgu.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gnajifldt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gvkmtsxef.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gnftfaqnk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/geqpaftbi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gcfxqijhj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyxahdzoz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gwbibngro.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gnbxzgwte.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gpgemixkf.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gubwmyhpb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gndyjpjyf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gyxlbgnxx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/grqduvsky.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtqgwwyeh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gsmyevwgf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gdeyyoeze.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gcyvohpmc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gatorlufp.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gfwplxdoo.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gmgpvargv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gsifglkvl.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gomvnlujv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gkwbxfxvk.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/greegidvd.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/goxgjcgvw.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/goapjsgbg.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/giwbaxfed.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/ggnfbgehg.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/ggjqbkerl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gfboroazo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvyradsjo.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gfyjuhjvt.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnsrluibf.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gdidbhris.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/ggwusssrd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gzcffrgan.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/grradcwdh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gecghhihb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/ggcmvnqir.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gcrcgchwn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gghgpqjpj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grynjoscs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gzkslnarq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gkuyucqpe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gmhnzpxpq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/geajvshns.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsiruonpm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gxtqyixji.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gnradzpda.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gznqfghcr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gtpasjeat.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gpxaknldj.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gwecshwvs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/grehigjtp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcrnpmrow.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/ghbghkzsb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gocdplcrl.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gluqhfbes.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/grmurozeg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbbjiohhp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gzkzwntbq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gymatzald.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gcebuzgio.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gjuuwdxjr.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/giejgmykn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmgyzrnyr.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/glgucpkwl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gzoqermzp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gwkxknjkx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjnbrzxur.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtattovlq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gbooazlqh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/grhgqcgfo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/giwxteooo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gbjzwuzhf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gokqydxfq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gglxvtgpl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gxbmblwgd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/grpohhfrv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/giztitaic.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gaoihhyup.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gutblkemt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gqyoreeyj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gsgufqaff.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gnmvubljr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gaelsrpnf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gmqsuyjrr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/grqepxglc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gooloehcf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gljpnojil.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/guflgyzin.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gznwdqstp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gpstbccrl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gdisjwecj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gftdpzwdd.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfecebwpo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwxcncuoq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gifozlmyz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gcpzkepts.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gaeajrbuo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnltllqkm.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtgiezeqg.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gbtnzjdcm.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmkmbevmz.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghltwxcuq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdjqqcfye.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gewupvzdv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gmbtstpjo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gseusezis.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnchtzqci.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqberlvvg.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gkfcdmbeq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gykevhdih.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gdwjbjvbh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gfoliuerm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gtawpcphb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/ghmwsseid.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmtbdaow.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gjbfssfob.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gsstypnei.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gzbofjwvy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gydwhtogn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gfgrusjwk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gwvabtigu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gesjtcfxz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gdnrhqscf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gblogjswm.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gfkegweks.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gcwtgrsrc.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gvalrmnej.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpjrjapzz.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/galbygrck.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gnqjclled.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gzggnqttt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gzbslfxhg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gyevpjjlx.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfufbpuoc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gfreewecj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gzygldcth.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gojncyqle.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpqmucwtk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdfsunqtp.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmbihjsay.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gjquconlu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/grdzdbscu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxyvmejal.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvppiwcpn.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gnivdpcfw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gladncgim.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/ggcflcxyg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghyxhhwjz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gsdzdqsem.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gvgfskejp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gasiwakwv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnsftmbol.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gcbhpwgpy.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/guxjyccak.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gkhqkksoy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/glbatccqe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gpzsrknmb.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/grefajmfe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gavoyxyff.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gqulslqgl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gcvqdjrjm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gcldbpunr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gusrenzxn.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gdnxjjnod.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gacmfvijl.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gkctjvqac.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/ghkhnwoml.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gtywtpttd.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gmhbxdbsw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gosoiaukh.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gsyrivwin.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gvgicowtk.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gpxuqeqhn.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gluftwivp.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gqevblwju.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/ghuktbdaj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtqeeashz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpidpryrg.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/ggfercdvb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggczwrzaz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gpqdfgewa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gaougpojf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gjacnvdnu.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gvwhmvffx.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gzjnpwhgp.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gvjpcugew.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gubyepfln.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/ggvmvxtln.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gpkwxgyqg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gbbzzjmra.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/ggiizvjyc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gpzequrwy.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gpufipqgf.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gjfpcjsuo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gevrfifza.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ghdqdufdp.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gwrgfjujy.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/giytqkpjh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gcvnfbqqp.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghoqnmivy.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gvxukwkwa.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gjteoxsuo.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gelnecohx.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gixyboffk.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gwkdsfprp.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gnrlxwnlg.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpnyjjdqb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gmxegnyps.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gjhzrxbvi.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gkegpafbb.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gzuhwugqr.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gafcvzmzq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gjmaityte.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gpwduvtqc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gsgzubbhd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gjlojfkgn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gkyuvyrvp.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gyhrodwgw.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gjfjxmavt.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gozmwvsfl.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gbulzcawu.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gumihtzrr.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gytzjuqcu.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gpxdmhlxi.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gszdwydry.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gqadskcfn.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gobwxtopc.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gbmtikvyk.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gbgsbysea.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gdvmtxvnc.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gpgyzhoea.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gelturinj.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gznyagfjx.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gjvbighyg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gdzoflcsk.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gonfpcuhx.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gnnqzsngg.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gilostdrp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gzpmkhfnw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gbxglrdrj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/ghsytabps.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/grrffquxt.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gotbhiwoq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gitkqqiut.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gwcpbjieu.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/guuelwzal.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gksjxcwyg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gnkbuikxn.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/ghujpruvu.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gzteqiwiz.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/grxualoru.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gfsioyelp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gnewmcaaz.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gewtjnkmp.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gbntacpll.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/glcybsfgo.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/grzeyrzpa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glxvwoymx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/glthxmjlc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gdefvdywq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/grkvwwdav.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gxyzdmbea.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gsuhkclsb.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gdcaeflnl.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gpeuvbshr.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gfjlgeedk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gbzrsoinu.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/grxspyfhv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gyocsbqhv.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gpnppxmjq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gxteyyhhi.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gwfwhqtbg.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gumoxqsrg.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gdwbwxaqc.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gdchkmiuc.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gsjghkfuu.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gstpkjtzh.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gytsncglp.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/glrmuxthr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gbeaqhwwz.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gukttouwa.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gbxfiyoxe.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/giudwmofe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gudmntnss.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/ggwwxoqfv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gqzueamkz.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gxaxaggrk.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gvjqjevkv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gxagrbgjm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gtfppdhcd.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gmgbzbydb.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/grwizskqj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gonetjzwy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/glfnvpfzj.sHtML


<!-- 参考信息 -->