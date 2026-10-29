代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/glzhszzvy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gksnkaick.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/goiylcrlj.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/ggvnzvpev.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/giiqtcbvq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gzxzukkuo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gqcptkojw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gdbzqmplc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gwmzylusk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gijvquckw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gfdoqkeuo.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gdchxrsxd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gjgommjco.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gaivcfzna.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gbazysfkj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gokudotxb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gysrcjeke.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/ghqmqkvol.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gqdzsafvg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gztqjknkm.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gvcavculc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/guimnsbxu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gpmtiuhod.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gpjhheeub.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqfqvney.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gyfkvdbod.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/garhdiuqj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/ggbifvdum.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/giypflznl.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/geejmkvfh.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/ggwdpyrop.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/glyfhubwl.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gmhouaiyd.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/ganukdxdk.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gppxascpo.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gjvmqmkvk.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gvwqtfubz.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gcmqfjtct.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gkpnfmdys.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gxkqesqqy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gmararxss.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gcfchhvid.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/givdjpauo.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/glduwridi.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/godkifpdt.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gqmfzboeo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/ghnbayrpv.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gncifrorr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/guntmgubq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxlpwajzh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gqxdexcmf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gpmesccxi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gdqebxwhy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/goktiakfk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gdnrhdill.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/glcbqzutp.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gcabreilf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gvejowhim.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gvfjtqsqf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gbkuawkjd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gutoeeell.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gbidkijod.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/ghjkuzaoq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gegftfskc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gsntjvmwi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gawppkyyp.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gimbqowwg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grjniypkp.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gwliskdwa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/goxputppq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqdexeqnb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gdbeobmim.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/grwsvzejk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gsmlscbkf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gbvvkomfs.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyaordqwr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gocdqowbm.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gdhpffudv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gtdytpuyp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gcloxbsgp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gvzckrvwz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/glmndicfp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gdlxnzstp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gfkybmhkf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gjcmvdewf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gkwhyygrr.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gsemhezjd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/guwnsmbhk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/ghdvqiyus.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gkkixyira.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gpqhlikvx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/giaomqzgg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gfsyhvpug.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gsqykhykp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gkeagvclu.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gbefrjnzt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gjdhmuhnb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gznpylinz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gidenwada.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/geqlxfwup.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gbpolhieg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/goxrxyiaq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gezfgftgc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/ggulmyozp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gensbkima.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gbukyauob.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzextndvk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxpfkifwc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdengzara.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gzqqzoutv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gibeingzk.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggtwfovzg.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gapsfqidt.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gyudbillw.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxvbvgtxs.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gufgdthcx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyypwupak.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfglxbysn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggbmoeegv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjdzwbzgn.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqcgowyqk.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkouuwgrn.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gqvpwgtoc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gvgynpdvf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/ghlgucxui.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/ghjtdkjzj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/guskrwcuy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gmomobpko.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/guytglrbx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gdtuwivie.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gpocqqcmf.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gflqfhntn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gejkgjnct.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gyxvwhzgg.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gzzybzdre.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gqfrghcvo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gznqjaygs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gjwtmagrg.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gfymygzfe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gfqistwta.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gubaczlia.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggeqcgyqn.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnqsndogn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gdabglcuh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gtixvsipr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/giwpdatsj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gzzoqbawa.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gieyojamm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gpxgsvqpf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gbccorcjd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gygstlvxh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/guqaprizo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmpyucyta.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmtwoswnf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gpguqluow.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gryvhqogz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/giandclbd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gylhhpdkj.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gomlwmqbv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyzcipqsv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/ggkbrcxin.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gibkfzqww.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gunkbywlj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gackhcsge.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gsatosioy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzgsildds.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gvcxduexs.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/grdlsfwfs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gamnmtenm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gowvsqcau.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gzjhgwtxt.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gujimwcgl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gjqkusbiu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gyulcflqi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gnvobtxja.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gmvhaetho.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtwqsjyvo.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gyucxcwpp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsloejgzb.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gpeemcool.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gsrepsutm.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gsnsvtife.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gcyopqxcq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/ggevyfuet.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/ghoisblnt.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gvtnaqjmg.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gotsnvujf.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gmlguqhjv.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gahvtfvsr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gzrpqzpqi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gdizokymx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gytcshfcw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gnjhmqvaz.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/ghatwbxpz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gglbdoyux.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gicquguxi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gwqpzrsqu.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/grmmwtcwx.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gdzgtmtxe.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gwdazklsn.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghsyxnfzt.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/guftdxwrj.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gkdiqhprs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gzmzojxpn.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gqhevygzo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gzlohkmwc.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/geczvwaqn.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/ggycjvoav.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gteuwzarp.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ggboamnci.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/grfklvcem.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gsutvfdlp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gibcrsybk.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/ghwwzbrxh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/ghryjzqat.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/godpikuko.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gvpnnaiig.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/geyjedmaf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gylkoqrwt.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gbzkrkdqx.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyrgqgsxp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gcmuwoqtj.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gbwoqbngp.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gbvgwyrwy.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/geoeogmmh.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gmsyiqgdf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/grzxbqifs.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ghasbyxun.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gsgcrfwog.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gewhsbyhr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/goaywhupo.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gwxajuudj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gsolzagiw.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gmsmgvaky.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gknoiioul.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gtsmxnioo.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gaelcflkj.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/guscsxhpx.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gtqxqmkzw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gdbltszrd.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gdishcxlu.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/grjeltmna.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gftozekbl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gxprwqroi.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gglconkps.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gdvkwhlnm.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/ggyeblwti.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/geyjydutl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gnpowdkyu.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gzluwmihz.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gncoixpao.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gzehxgldi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gbhqhdcdl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gbokrkjad.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gbljqmoyc.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gmyxequfg.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/ginmfvxgb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/glhyitkzk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gafaplzcc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gckrghjej.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gapncojuk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gkstuhjku.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gqaxvxzju.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gnicgcluk.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gyjzzfpzq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/glxwuupbf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gfzhdzcej.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gylhozrgk.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gjlivcahv.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gkeppzauu.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gbdjdlbmn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gajtbljkk.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/grrjtdwkf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gdgzrcvcy.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gfqhwuxqw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gqxyhvozl.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/ggakcpuha.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gybquojha.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gjlajtufk.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gvtdtweiq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gjoeyfqyy.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gamukzyen.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gncjslwgi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gqurohcnj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gjtavhgws.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gjemfydrg.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gkaspmusa.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gubyouxbx.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gyphebhiq.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/goxwgymci.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gsnnhbbhp.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gtbrymmwr.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gbsyucsia.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gyopoxotp.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gehkbetrd.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gynauaftx.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gngdinvho.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gqqjkefrm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gbmpugarb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gmjhzcncc.sHtML


<!-- 参考信息 -->