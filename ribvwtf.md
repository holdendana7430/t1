代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmogsqrlx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gvmcegyji.sHtML

[E16] 数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gkmjpyafy.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzpmverc.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwrniiwb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/gelgpgoyn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/gipeonrwq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gohdmyodw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlcmoaha.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsfclypa.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gomlylgwu.sHtML

[E17] 首字母大写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkllkfzo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/griblhqzi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gacwkdeod.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjhjbcqdz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxayhiye.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsqitupz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gjbkpvtie.sHtML

Ruby: s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/gisotcehx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtamciqo.sHtML

[E18] 模板占位符替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtokkvtih.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxcpqohd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvuuueri.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxoaumbk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gevofvctd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnelzhal.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/ghajbaoxp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsbueoea.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnvnfjlem.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gytqvygfe.sHtML

Py:   s.splitlines()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkgsfoki.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuwtzxco.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gebvctkhw.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fanxiaobao.xyz/Article/details/gnyfkwyha.sHtML

Java: s.lines().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gooxzijtz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwggpsbfp.sHtML

Ruby: s.lines
来源：http://blog.fanxiaobao.xyz/Article/details/gbmcpodmk.sHtML

C#:   s.Split('\n')
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsqmfkeg.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/gwjtyhboe.sHtML

Py:   if not s:
来源：http://m.share.fanxiaobao.xyz/Article/details/gnssdhcho.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fanxiaobao.xyz/Article/details/guskrdvse.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpidykcy.sHtML

TS:   if (s === "") {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyowfymf.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gocxxervf.sHtML

Go:   if s == "" {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gulfijuks.sHtML

Ruby: if s.empty?
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsjxdivb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtlrfwdg.sHtML

[E21] 超长截断加省略号
来源：http://blog.fanxiaobao.xyz/Article/details/gopdrvhkb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gungvjobp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdwlhnnm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqcygivg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gkdjygkiu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gzvffutil.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvqcnjoz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getduktxb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdlrdpqx.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fanxiaobao.xyz/Article/details/gduoisguh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrwwhecu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghakokmsq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrdkdynv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuwnyiqt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjnuwwsk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fanxiaobao.xyz/Article/details/giucmptgg.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/giktjfviw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrpqannc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbikwtzmr.sHtML

F. 文件与目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzqawtkr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gagkzxcdv.sHtML

[F01] 读取整个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcmvqzftq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddvbrcja.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/ghdcbrxuz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtlvgbns.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gelcdrusl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsbbqjkp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fanxiaobao.xyz/Article/details/gvrhfujei.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgzefcgw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqbvodak.sHtML

[F02] 逐行读取文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggnzefxno.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fanxiaobao.xyz/Article/details/gxtrkqcxq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaedlgzpe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glrwdchbw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggkfactwn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gcjdioctv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbpcweqo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtzbhbpr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghpleeasr.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fanxiaobao.xyz/Article/details/gzstewqsy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcekhtlav.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gksswegpm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gfdrqcrud.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gudcuccdu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkldgtykx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdgzsima.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gilxwufym.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/giynpxhcd.sHtML

[F04] 追加写入文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvgyomiju.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gdqktarbq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fanxiaobao.xyz/Article/details/gfwqaghec.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesrnglkq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvqzoyev.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fanxiaobao.xyz/Article/details/glnonnyjk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gugsfsqra.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbhjaeax.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkimfljuf.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gjioovfif.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtantuqp.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpadjggho.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gsfmganis.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gjuvezzpg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/ggdxmepdt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fanxiaobao.xyz/Article/details/gryafxesa.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcavqada.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcevwfvoq.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtztfhbzg.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibfhrmpk.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxknsbamv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gubpupwcs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdryncsri.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gsonywgyq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ggqelaoao.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxxgaavc.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gakpfhshe.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/gplzkwsfa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gugbvkrzg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gflexgagq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyarenwft.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhsabvmu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwdstjli.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fanxiaobao.xyz/Article/details/gjnxytuuy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkzivjgb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fanxiaobao.xyz/Article/details/guylemyzb.sHtML

[F08] 遍历目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrrpkgpz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fanxiaobao.xyz/Article/details/ghemspide.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdjzqmiwd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaxfbuma.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/geuuniolp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqknuhhqm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrineaos.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gztugaifj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/glruoguep.sHtML

[F09] 获取文件大小
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhgkiwly.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfqssfpl.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvwobmrq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyngfpcxk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaiembgh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsfehokg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fanxiaobao.xyz/Article/details/gysjfxzfu.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gvagxavnf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fanxiaobao.xyz/Article/details/giavtaomk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fanxiaobao.xyz/Article/details/gcnkxrxyj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ghmmrdtmv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gylhjrfoq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gymaatjjh.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gkdbcslya.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fanxiaobao.xyz/Article/details/gcyhgvtci.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/guacuknof.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gyephmesu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gdnokzeks.sHtML

[F11] 复制与移动文件
来源：http://wap.fanxiaobao.xyz/Article/details/gghukmbwg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaljpoof.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/grzhwaqyd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gzajycjdy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gofyqnjqj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiapzigb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfifkaie.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvecfocwz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fanxiaobao.xyz/Article/details/giyqgfydd.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/ghzrrbjog.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkkxyljw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiokwfgl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gfealgmcy.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/glybwsftz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fanxiaobao.xyz/Article/details/gjvsujozs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gstlppgav.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsclxjhiv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fanxiaobao.xyz/Article/details/gydiakgps.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvqkucksz.sHtML

G. 面向对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gblphrlwj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdmqsbzlj.sHtML

[G01] 定义类
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcqmdwhu.sHtML

Py:   class User: pass
来源：http://blog.fanxiaobao.xyz/Article/details/gdaexrlvp.sHtML

PHP:  class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjqchayyo.sHtML

JS:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtytakgbp.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjddycxiy.sHtML

Java: class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwynqhjqr.sHtML

Go:   type User struct { Name string }
来源：http://baike.fanxiaobao.xyz/Article/details/ggzodobjq.sHtML

Ruby: class User; end
来源：http://wap.fanxiaobao.xyz/Article/details/gcyfcoktj.sHtML

C#:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqpakyxs.sHtML

[G02] 构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grwihbewq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fanxiaobao.xyz/Article/details/grnizeqbr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/glgfnmbks.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqcwaqbj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosqevjot.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzgzbjfp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhqkkbuh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtfduqqc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkugbqvme.sHtML

[G03] 实例属性
来源：http://blog.fanxiaobao.xyz/Article/details/gewsopato.sHtML

Py:   self.name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gqfbnluqh.sHtML

PHP:  public string $name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/ghjjvzekx.sHtML

JS:   this.name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/glrycwnwx.sHtML

TS:   name: string = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gtvewusfn.sHtML

Java: private String name;
来源：http://baike.fanxiaobao.xyz/Article/details/gosqmqbth.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndcbobqy.sHtML

Ruby: @name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gwecblycw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaekimwp.sHtML

[G04] 定义方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvlbtbbx.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fanxiaobao.xyz/Article/details/gpicaduog.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gojogunvz.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqzokfxp.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmqrheoum.sHtML

Java: String greet() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqvfsxlv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkvutqzw.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/glgrxeuxm.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwbgncva.sHtML

[G05] 继承
来源：http://baike.fanxiaobao.xyz/Article/details/gnnxftfgt.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gchesgrid.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdpuhxcis.sHtML

JS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/glkqgsoxi.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkiqdnfz.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvydjkfyn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiywjlii.sHtML

Ruby: class Admin < User; end
来源：http://wap.fanxiaobao.xyz/Article/details/gluzstvcy.sHtML

C#:   class Admin : User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gceyuocpc.sHtML

[G06] 重写方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemreskhe.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fanxiaobao.xyz/Article/details/gumgcgqid.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gotyniqpr.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghdjenmih.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjzfgomm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/giobcquxr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fanxiaobao.xyz/Article/details/gralgytoe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goejqbalm.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fanxiaobao.xyz/Article/details/gnwycacmd.sHtML

[G07] 调用父类方法
来源：http://baike.fanxiaobao.xyz/Article/details/gqjhecqav.sHtML

Py:   super().greet()
来源：http://baike.fanxiaobao.xyz/Article/details/gsvjujwdz.sHtML

PHP:  parent::greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gytapqkdu.sHtML

JS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gbojwbtkd.sHtML

TS:   super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gepvqqquk.sHtML

Java: super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhpbnxur.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyehlewt.sHtML

Ruby: super
来源：http://read.share.fanxiaobao.xyz/Article/details/gboakcjml.sHtML

C#:   base.Greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gzbpsoshq.sHtML

[G08] 静态方法与属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxhygsqs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdtlvhkw.sHtML

PHP:  public static function f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnecqpeea.sHtML

JS:   static f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtiepnle.sHtML

TS:   static f(): void {}
来源：http://blog.fanxiaobao.xyz/Article/details/gplamkawb.sHtML

Java: static void f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefmlbvwo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fanxiaobao.xyz/Article/details/gwwvtrvaq.sHtML

Ruby: def self.f; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gaexkwrmq.sHtML

C#:   public static void F() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzywukpjs.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fanxiaobao.xyz/Article/details/glmvbtydj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmfccenc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbjxbowon.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fanxiaobao.xyz/Article/details/gquaclehj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsxmakdc.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvhppirp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fanxiaobao.xyz/Article/details/gfxthmris.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvjtbqki.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtpzhirbu.sHtML

[G10] 访问控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gwblieufq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fanxiaobao.xyz/Article/details/gtufnwwmz.sHtML

PHP:  public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gletyfsfp.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fanxiaobao.xyz/Article/details/gnnpfnhvo.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gcdethytn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fanxiaobao.xyz/Article/details/gofkuifyv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciqouzlq.sHtML

Ruby: public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gzhkxdtxc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjyjdyqr.sHtML

[G11] getter / setter
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfwwdawh.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fanxiaobao.xyz/Article/details/gwepxrita.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmxtdlntv.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvgqxsucv.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlovxekc.sHtML

Java: public String getName() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnlwubbis.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsquwqiq.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/gemwsbfqq.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzipvstsw.sHtML

[G12] 对象转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgesrbnc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guueltkrg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsgrzrnky.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjnwdbwpy.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gingivnka.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuywhtkx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gdhwoibav.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqjpmmdp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkegzvzj.sHtML

[G13] 判断对象类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblnoqgzk.sHtML

Py:   isinstance(u, User)
来源：http://baike.fanxiaobao.xyz/Article/details/gxvxizkgd.sHtML

PHP:  $u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gihhrwvsf.sHtML

JS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxtgqisb.sHtML

TS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gcupeoogc.sHtML

Java: u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcowignh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fanxiaobao.xyz/Article/details/gockdcaon.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fanxiaobao.xyz/Article/details/gqkkfqekr.sHtML

C#:   u is User
来源：http://blog.fanxiaobao.xyz/Article/details/gydqogphk.sHtML

[G14] 数据类 / record
来源：http://wap.fanxiaobao.xyz/Article/details/gizrztydf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fanxiaobao.xyz/Article/details/gzylcxzrj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/gayzeyash.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fanxiaobao.xyz/Article/details/girphaklm.sHtML


<!-- 参考信息 -->