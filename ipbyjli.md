代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gdgkmvivu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gketyiwxf.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gmznggvuv.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/ggdyrtisd.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/grynsvhym.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gxisdjjpf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gxrwiprlz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gybqtbqgx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gkwpbqjmw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gzzafmljk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gmfogloop.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/ghtkcwqod.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gfzwrrcla.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/ghqodrwpa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/govhetdkg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gvfuxfbvg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gulbvlhgc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gndacfymr.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gzszpwzxr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gblfgcqvf.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gednneqbq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gzxibndos.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gzlyflxwv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/grhinqyfz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gemiwjqwr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gedimuqwf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gandrpnad.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gxcqeyvjq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/ghpzyqkzh.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gklizpnqg.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gayrayaak.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gllfujcwp.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gmgmvhjon.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/giogcdsch.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gdqpqzffz.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gfufmphic.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gsvesnoes.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gaglubzle.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gdzebmdrw.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gquxvyegn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gwwzromcu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/glsfddyva.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gtisoqpvv.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gdlocutvc.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/ghyekvqob.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gazjlfjfk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gkfcuxopy.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gvrohmqev.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gqnxspgzv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gyjvzlohn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gxmdosphd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gfvttrpjo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gcqzmpgjg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gwtthgqze.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gnwztzidw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gvnmygxsu.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/givgqyipu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gvoglurht.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gudmijggn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gvdfhbegv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gcwcwpeki.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/goplkuoho.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/goofwgmmz.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gxjlbabsi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gmygpming.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gelmiuryt.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gqzjnrpzs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gskwkzhea.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/ghosleyur.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/ghgfaomjt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gopvywpnk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gvdwyndhe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gruaiwvdz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gckepkonf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gvtvneblq.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzhzcniif.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxmgyzvgn.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gfxiyufor.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/grwjfvori.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/ggtjalfvc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gspgqhpme.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gjkhiozgz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/ggowkreju.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gggpifran.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/giezqiczv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gdazjgvhh.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gpwkzvett.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gzbygbjap.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gvmgrourx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gcdcpgmsj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gfgojvony.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gtdlvhprb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gbeetjngh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gycrctubk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gaeayibcp.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/ggoexjeft.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gabtlundj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gajkldiyr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gmbupdfpg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gxjpiwhfd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gffkxcrhb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gpaeazxtv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjnrozyb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gubsbaewc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gjuomxqmy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gebbvwmjl.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gikwglkgv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvjwshxxo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gaspyqftm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gxqnifxmt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gvwyzpznr.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvarwlodi.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grwsdfalz.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gqcwowmib.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxllhryjh.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtyqlakgv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcvpqvdkb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwkvhcytz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gonvwoezk.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsmuqcocs.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqzjsdyee.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvgqsugme.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gwqbyqmfs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gqmwfbqaj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gelnjonra.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/ggkgenrmt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gaanxvpvi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gauvxuafh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/ghnchfrpo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gfekhqxcl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gwneurdqj.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gmrelimop.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gjtgzrkmt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/giothcgid.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gnudlizfr.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/ghmbvhrmn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gvshxnzom.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gqyukoklj.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gpdrlhkhs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gxnvmeqph.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gefetrnle.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/goxsjusic.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfcekmhsc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gxcwltjsi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gduhqfmxg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/goruhrcks.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gmtabamrt.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggloyxanx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/geimuedzx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gsnuzosbb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guxvowdso.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghzzgfxbn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gskefymha.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcmsmsidi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gosxhyceg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxfhxhbhp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwtrkosvk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggisxzaav.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gfprxaajm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ghvyogtjp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gozusqhjt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gocauwsct.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/glsjczeiu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ghbdbeehr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gglxezclf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gmcogatgv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gausjyqkf.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gvjoefoju.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/glmryxkcj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gnugvjmtg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gkpuyvhqt.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gamvbtfdu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gztivjjhs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gtcvkvpnz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/ghqixwnzk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gvjwwbiva.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxyyivwkj.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gkttyaddh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzehepcrv.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gfrnmtqpy.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gpktlfrbb.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gvmmqwmdi.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gnzulcphs.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gmzlvypnm.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpiioiany.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gomathdfe.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gvoyognlc.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gzwtnvwkt.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/goojwigey.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/grxegcwny.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/ggvlgicft.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gkwnhfpbk.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/ghmeggoks.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwppiaanv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gihlcotxa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gymmxybqs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gigmloxxw.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gbdixiylo.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gtphylvps.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gudvirqlk.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/girvlowld.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gxipafloz.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/grdyzcrhs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gmzcmbnrk.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gpwsnzxen.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gquhcrfkg.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gtbhzyevn.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gnybhlbal.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gjdjdaoay.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gpsugnnsr.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvvviucqm.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/grhnvrepm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gllpprwth.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gwfvbtqkh.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gosvmmimy.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/geaerfsln.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gdhijwrtk.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvmavamst.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gsmtuvuch.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gmtzzxwcu.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/govwxslmv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/ghivxmjas.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gylgqprfo.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/ghdjssbmx.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/ggnxlemiw.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/ganwmiwuf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbimutrqx.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gqdcsqbgs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gjouboukc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gyawbwxjo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gofcjbhoi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gwmdymrdv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gfeatlblz.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gipcgvdwa.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/ghmnbtvwf.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gzwkuzdwb.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gjvuejeux.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gguebfhxb.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gfbwnyokc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gxjycnygs.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gytyzfeya.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gwoztiroh.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gaswioeer.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gtptztzou.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/goxmafxxq.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/grkjlumgq.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gibwwolfa.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/glxelykgm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gdzdxftsw.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gwfgecjxn.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gzlwkwoqp.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/guuyynmhb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gnhddvpus.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gxxhbexqt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gljhntvfe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gqqlojtqg.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gxkqckqgv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/glssqoceu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/glmzalkrm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/goboqnbqq.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gahsitowo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gymlbebfj.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gqsffcgka.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gejhiihku.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gmsxrptff.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gpxrphhbg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gtmprrugc.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gjuuiohsn.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gghphivqk.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gsaucdfak.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gcskcjowp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gyvtasjdd.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gfcvqvnzs.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gjhlljjfd.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpjvxodve.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gifrtpyrt.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gnvdkmfyh.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gjmakeuqj.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gpwjjwciv.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gmmgigcgn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gkvamcqyy.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gnswlgohx.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/glibwhnjl.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gmimjteai.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/ggzldmhfw.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gsafmxnaf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/goxsziobr.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gkqpqclll.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gdaedyqll.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gggqmjrnt.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gekjjbfme.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gjvvtjsot.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gncpvsqcn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gngmlttmi.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gupuncgqc.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gbkiahwdi.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gggbxvacz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gjwpebejn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gmkaqsekn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gquabionz.sHtML


<!-- 参考信息 -->