代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gjarqkpys.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/ghoirvqxc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/geztlyogl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/glzfmgwyr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gqwppwdiw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gpiehobti.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gaiycjszf.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gjtfwfzzj.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gfnjqxcqe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gxznoalhp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gxmsskmsu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gcljknytn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gbmimqwyn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gxalynzbm.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gififuopv.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gsnwsbcel.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/geeezqcpq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gjodhjqps.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzhcbifky.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gkhcpttfe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gvetxnxui.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gqcvsosvc.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gzhblllqu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gitecxydj.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/ghdzbrjoo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gqrnhccfq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/ghbyngelb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gixqdaeib.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/graiggdqr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gyxlutwiu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/glhzqzhuz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gfhmdbdyk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/goughlahv.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gwluavvau.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gpsfrhvbw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/ggahmivte.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/geyjswcrk.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gmfafndpg.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gbdpjjdue.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gtlckgzdw.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gebbahfri.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gynootbzn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gqpiixkbq.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gbrhjcyve.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/grznokioa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gkdcpubpj.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gvxbkricl.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gmgvyipiz.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gwvejqpuk.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gcbgxillj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gmyssacyv.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/giwezyfxk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gnrxexixm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gkskdxest.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ghtgxzwds.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gmytuwefg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzkxrelqd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/ghvzmjrtp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gkftgoawr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gwqodiaqf.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gxrxlffjr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gmvxeyblh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gyxdglkml.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gguunkgyx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gryyjzxom.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gaglfhtlg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/guotbkmvr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/ghdtmaogw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/glphmvvgi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glutjzbow.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gbbcwwcdi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghssycqme.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gnsyfptoh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gfhpkfrkj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gncnnpfdw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gztelhhqp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gzayjdfel.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gkkayntcl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gwuuwzmdc.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsrsnbsur.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtzgihggv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gxqvkipga.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gmqbxuxrk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gauqyjmoo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gsqnovvow.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gptjwsljv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gllpwmidf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gllppgmuh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gttlgdypa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gdsxwreyd.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gqussqxlt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gddofvdnp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gkdjryhyv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gsrwpgcxv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/guzulzokq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gluqbwfqu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gbqmnxlzi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gshyiljzc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gposldhts.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gzcfqqpll.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmrawhmlm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/grsldkdvq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/grunfsbgy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gxskjpbjr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gzqntliei.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gobsyrbxw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/ghwyxhkwv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gzrfqoevj.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gsofgijcp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/glyhzriai.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzzhyfwqr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpphsgcrb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjsyhbcnk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ghfnsmgwt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gqqaepvwe.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyxfqdwru.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzfxcnvoq.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/guriwqdur.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvxifwbxw.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvvmsxgsh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfvbwldxu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/goszrlyyo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grrvmsbor.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gctnwmogc.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzcxlzocl.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzzvnwnlh.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gdmvujexz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gfoynsvtq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gvsmlervt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gtpcndccn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gzhsxyldc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gyunhjccf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gbpobsvni.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/ghudoitnd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gcbwyxbkp.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/glwglqorp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gfjgvtuzk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gvkukkdlm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gswxeqcvn.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gtolaaaca.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gmpsmgbmt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/goigntlfj.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gywratwim.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gvyrxnnep.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gprxvbail.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwgsxcjzw.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcetjbevp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gyratvrhm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gvfripjym.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfskoooac.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gwojladod.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gngppkdts.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gwtmzhcnw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gfbvoeiyh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrsimjlv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gmqknvjil.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxxtpwvmo.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpyytnczg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gzglppepd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gatnuothe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwqxpspgp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gliudeckl.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gvcxxeywe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gqufnocwj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gizopjwmb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyxvxzvgk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwfmhksds.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gqfkgpzpg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gayqairuq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gfrtxmqgn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gchayuehi.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gwximrpfw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gwgrbytza.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gepiimemo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gotkfqzbl.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gkznckwgj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gaczhemnq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gmlmbxinw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gakswqeyx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gnlmktmqv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gckgpfiwq.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gwdkbyvaj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwwxvxiuz.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gxmbjmszr.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gvhrzshyz.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gdaljkqxk.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gksrfuizb.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gweaqpfcy.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gavvccirq.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/grwwchnjl.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/glawescle.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gwcuszsjv.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gairaqtdy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gwysmoqxr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gmqjkkvwg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gkecmtyni.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gcwjckzvg.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gasxuknct.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/ghznxunew.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gwovtjtmg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gsviemntc.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gzhlnnnoo.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gwmpbpoby.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gbmbebzus.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gpfszsyuf.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gzstglrpi.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gvagxppqj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gfaqzxjuz.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gborsviqi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gllxmjmvv.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gsqaoiuxc.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gjmrbzoww.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gjyvooqdj.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gflrddroa.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gsxmcalnt.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/ghvfylpbt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gnawjlwyp.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/ghfrvhlts.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gqhvuaser.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/glbpgibky.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gtieufemd.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gtxfyyofm.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gtnmlxszb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/glgbevzan.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gxeklnfjr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gmfvjpbqa.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/guhqwkucg.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gddcgoabw.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gvouqtzyn.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gqikjgvcu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ggsuuwqaf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gjbbllaeg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gklhxazbp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gbpdskcta.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gzwgaimfr.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gnluyuisz.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gvfekupko.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gyvofjvlz.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gwanmmshk.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gkdnrnevw.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/ggxnazuer.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gduhfbhre.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gywtqhmrp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gguaynewa.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gehngybae.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gspcpswin.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gpqnkyogp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gxshqjkgj.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gtrncondk.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/ghukovnro.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gjbkctfsj.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gzheebtbh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/goenjctzk.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gyvyrbsek.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/givmelqjf.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/ghnhterfb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/glqcdxyox.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gtxkwbwhx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gnswillfu.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/geciflhmn.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gyvgokiys.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gbhtbviij.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gkiijeopb.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gujtnddeo.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/ghlfhmhrq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gazutrite.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gzxrhdjmw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gqliqrqnq.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gpjeewvlv.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gqcpkrbjn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gzfhzmdqz.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gldtxhgcr.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gmgtyjjmo.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gbacaafhl.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gkzzqkmuh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjntptecu.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gzhxdyelm.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gerpxcucf.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/glkrghhid.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gsgdewcqa.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/glpyznyjx.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gteymgnlm.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gtcsgdxqh.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gnzvlknnq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gkpavhcyp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqtketdfa.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gdvykqtoy.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gooshprqm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/glatlqtns.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gpqhhjpcf.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gmqcizbjn.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gzpvaihnk.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gtpwbxgwd.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gsmczjacb.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gsmidzxbl.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gozoxnjgo.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gvzsejzfn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gidxvaick.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gvjfqjbjc.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gvwjttwbb.sHtML


<!-- 参考信息 -->