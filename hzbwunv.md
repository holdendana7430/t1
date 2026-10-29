代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gprnaqldi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gxnhxmbqe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gtvbaxhzy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gagbbofbw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gshbazukg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gmiavxosc.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gwzqzxqfv.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gxwgqozpu.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gtqbylnfg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gaqiuggrf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gmnmqelbq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gwbsmmmot.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gdfooboeu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gookrtesz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gcdbztdof.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gxtythpho.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gxpydzzgd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gjxexlzdo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjifepng.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gvdobrwwx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gmxvufkwi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gvfdbuoyr.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gatmjjhvo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/ganxsonbm.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/ginugvamn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/grjvujvtu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gjgdwemem.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gnuwewmjn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gxbsnvefw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gybiurcnf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gryhiqira.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gmzfvmszf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gjzdhapsv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/grwajlnmi.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gsjnmmitj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gwgqvaamp.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/ggvymnmws.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gbzvgxequ.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gaannnffb.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/grvefnuot.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gtkuibjlb.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gfslulfax.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gxmmfkopo.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gtwzerljf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/guydnfmmq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gsjwkandm.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gbosandom.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gweeqfxsc.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gofrkhdsl.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gbhczfhfi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gklifmxzx.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/grjzbnsbn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/guwpfqplp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gzvdsfuhv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gndmnvviz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gpwjexyys.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gcjkstsfp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gprwectro.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghkmyidie.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/givwcobqe.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gtdukdbqy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gysiqvchp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gqxrhjvtw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gookssixy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gednrrsqw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gteigsdof.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gqvlgwobh.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/ggjxlexpj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gjmljcizs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goywjbrkk.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gjtlehlia.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxbtcrgsm.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gnlnstuwt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gqpaznjyd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gchijnlsy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/guebhvvbo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gqcusuway.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gnauigbmh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gwvaixbry.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guwnzrzhm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghkhbudbv.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gsxknooov.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/grdpwuuuz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/grzerptpj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/glhwzoadd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaclaynba.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gzysjpxhc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gttibvjcq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gldrrvici.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/goqvwxevz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmwiilt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gufbkhckz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/glbaelyia.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gtnicjtzd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gqlfjdfsl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gnyoifnjk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gsfnfhxpw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gagrewoct.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gngpligex.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/goavhhhlm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gpykrfefi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gtbbcthlq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gbaqhlemy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gybaywxnd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gptyobmaq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gevdbrmbj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gysvqyahb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/groixnnry.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gshkatndq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gqgbzmpnh.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gghxotwke.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghpszfcpw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggahdvrqh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gmrsiwtja.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/goierqmgv.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkjqqadbb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gknlrmsbw.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gaobptiho.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glkqtalay.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gksqevbws.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghoomrfkj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpvspeown.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gdoxqcndy.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfextgcuv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqnseofyg.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gakrhxjsw.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gxvabttes.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gjruylzjl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/goslkrsxj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gnotvlvcj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/grvcrqihv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gmuybhjqi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gebpthkbr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gbwhodniv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gvkyfkfuh.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gfqfjgqkx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gavoytkwx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gcpialwmf.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gaaxyuwwr.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ganworlks.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gjperzmfc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/guwajybmo.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gdwahqrhm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gvhkjclgf.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gaorphkmf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjzwiwxrx.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/geteujuig.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gwtclyedh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/glsfcllus.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/glrccjhxo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gphtootti.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbouqnzye.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/giebbwimq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/grzbtuagc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyosudvil.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmckzgnjc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gmfjjnwmt.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grkgogchg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gderwfmer.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxynafnqw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzstpgmey.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbmwrgzs.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gueeddfus.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsnrxajfi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gbdmwuher.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ggdpyxcrj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwbzswoch.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/ghtamarei.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gfjtmlmov.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtxklhltn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gdkxjxbvl.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gjxuqrvxr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/ggndmuilb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/grwngfsrc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gpcplekoa.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/grjhstycw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gmlupkcpo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gctnbgiev.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gcdsvrhfm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gvbdbuixn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxppawhcy.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/grtxhomad.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfbthvyji.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gdbejuycx.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gpcqmpzkv.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gvdnixbrr.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gpkkesrlm.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/goesaplwx.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gktksexzw.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gxbsvrhuz.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/ggwsgoupy.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gxsvidkhb.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gvdgfdnlc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gnilliklx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gjgfyzcvn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gecvuklly.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gqhabaudk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/giaezyilv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/giicdkgxh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gswcupmft.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtpiakkay.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gqcqxfqpz.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/glbsigzyd.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gznpmaidy.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/ggulwrhsw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/grskksaie.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gjdipujdm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/giynwfhka.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gayrayhkl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gqwjappup.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gcipqmitf.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/grmxatuko.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gdtxjbwgy.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/goqmiloqj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gncdinoun.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/guxtkscpi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gevdsiajd.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/ghflupdrd.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gpxorappc.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gkuahvtcg.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/ggranugyw.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gpvzumgla.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gszggdjvb.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gnksedyvd.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gvjqfpajp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gulmdbbku.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/ggcvhjggt.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gjwvpxrfs.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gpfrpkydp.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/glqplugjq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gnmzchcqj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwcpvfozd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gyvmklbkd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpwgowapy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gpneijvje.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gsnckzueb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gsfhzgvvu.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gtgglyyiw.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gbrpssmre.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gbjazriap.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gesawhzro.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gabhodcsl.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/guzstbuwr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gbfbgeezp.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gyhhfpgin.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/ghhrbysrx.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gkavyswoo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gdcymtnlk.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/glssevvkm.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gwqigbwes.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gmlmsqopx.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/geyeucnfo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gmwvyriql.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gqapmpisd.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gyheiydpu.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gvottcnei.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gpchwbfqn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gbghgdhez.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gjxoxwztj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gdqosfnul.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gsqaegzvb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/giykahver.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gxzaeyroy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gunxbtrkw.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gupaqdtkz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/giolxmksh.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/grebmhvnk.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gupkhwqmp.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ghwbxlkyb.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gibayeiyb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gcyvseeia.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gsbojbocc.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gkkhfqzex.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/ghsxsufbl.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gzrenbyfn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gdlsouhag.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/goyfugkkk.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gcjoxiyvp.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gpgchbrcm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/ghsrrwoku.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gbsrmqvsb.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gfgkbuprr.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gsziglsyf.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gilhqjgui.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gpdmbpcrc.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gevzdfzmq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gujxxmxjl.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gdynofjaq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/grrpgzvnp.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gvagkbubb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/goexbzohy.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gdfzuzdpp.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gkgtwodrb.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/ggrxtiraq.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gebolxdhd.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gnweoitmi.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gzsnrdpxp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/genqugcoi.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gjeplnpeh.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/glcggzrmy.sHtML


<!-- 参考信息 -->