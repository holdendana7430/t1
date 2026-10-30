代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/grerkzbvi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gpavamajm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gzujowypc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gpysspexe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gbnjnmaqe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyjobwhnk.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gpvgvcqjr.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gyvxnayne.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gdjvqqgky.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/ghcsowixv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gloalkxlp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gojiwceeg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gszoxmdjr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gfigjlfcp.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gjkcirtzu.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gxbhploca.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gsovwtbsn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gmsxcovqu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gmxbrxysl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/giudemvwz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/ggobygwhr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gblkumzpl.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gofzykauj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gnntnmnsb.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gscjcnhkm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gzjkwdlrx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gkwkkubxo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gmndtqfdb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gfmwjhfsk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/getqaopck.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gqjeicnub.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gdtxzunpg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gxhwmmitq.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/guivucbsn.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gahsskpml.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gupqezdse.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gbczfhxro.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gfejktkmg.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gnzpktirk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gqcyiwcdx.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gssqmevrb.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gulvgyqux.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gcbzugumm.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gnvzyjeuv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gredokfmy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gifijgsoo.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gndpzxekt.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gdiifbaud.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gnwmvhquu.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/grjpesqsu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/guxhhszyb.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/ggaxghjwp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/ggijzaztq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gtjmlhing.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gmwjuxoor.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gfcukvsus.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gjvlzpqtr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gkmjvcbqc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/guuirzknz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gfhxyeqpy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gnngvwcdu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gleyobelb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gsxdfabyt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gdreglxye.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gwjcwhgfu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/ghcbcxven.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gnsnaenex.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gwqdnpozt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gxivjvwvn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyawfdclb.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gkqztgwdl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmxtymitc.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjanvugpc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/glfouuwnb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gvtdvuxsv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gvlwjiffa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gsvyeoylo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gogmpjbff.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gacaermai.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnareowhe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gorqzjrud.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gddflmwdq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gkgitcpxi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gkymuigdw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gxanntmiz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gdtxjetvz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gjmrufpnk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gqqxsdugr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gzlgtwtds.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gbtgtiapm.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gaqrhwwlf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gyagbxsfp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gkbfoivqb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gozjhahnj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/glhuoicbt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gryupevhn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gsrmbhuep.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gvchscxfm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/grugqddpl.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gdnmngrpj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gueiqhblq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/ggwqmyjqq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gaopsyuob.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/globmmatl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gdzykaoff.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gakrmjpca.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gfomfhqlw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gyoxhhytv.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gbacrtsuu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gtiwjqrck.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvjeynngz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjkpuygey.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glnkvvzvk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gyfrsyqif.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gxiksllzw.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gphgjopyq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gomcozvgp.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/ghegwzydp.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmytoruvj.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghsrmxrhg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqzrmhfyf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gczptrsfr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gfiafhiex.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqrtyufgn.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/guicrmxji.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfgktwyps.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gtgycnoeu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gipmrxgjq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gpkkpiuie.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/goctosodr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gzvapiieq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/guzojzzwk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/ggclwbpuj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/ggillafdu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/ghmidvdrt.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gpjxqlxxd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gqczjemzw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gacwyobxu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gesyxgvcn.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gtsxznzbm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/grzpfyzgk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/grkzgupqy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gnvuimvvl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gjoxundwd.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/grfusukit.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grpsryxhs.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gheyurvhc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gwrjiqqir.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gvuomjmpp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gtepjlovc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/glimzxjut.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gggihuebp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gneefumdp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gkskwzfrg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gftuynlko.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmuvnrhaz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gcxiynrwp.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghfxbdalb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gzoaqjvdd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnuuyoxru.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjfralkhp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyynpiptf.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gympsdbpq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gitewoepz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gjqrognif.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/guxdilbou.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gbjxmunpj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/geoowqhuf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gmmftefqh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtgpqixve.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gukimgpbs.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gcbbknzwy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gvokqnzwl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gunlrsupk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gbnyliduc.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gcveehouv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gdhkfpied.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gqoyjpkcm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gxebtpaxr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gfejudusw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqmnnrxff.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gjwukosfz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghwjtbxdc.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gsnjpddeg.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gcpylyfkc.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gbgehmcyh.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gxtbdxkwx.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gdiohjvoq.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gytxxseqr.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gojitaqav.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gcmolbkod.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzrttthzi.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gjwqldhbc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gqilhipxb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gbnbijfwy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gotlvzgeq.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/ghclqwlho.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gyimgvqrp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gkzlpyvgb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gpovfshwh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gyjxfduwq.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gbsmtonep.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gbfujassk.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gxfhdceyc.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gbeewrinx.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gzyvmntgb.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/guahzvrrs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gcryvhfur.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gkghmshhn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gkbpucmlz.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gohpnzmmx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gnvxepbpy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqsngbxgc.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gvkwwxcic.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gnwibmzqp.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gakdrpkev.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpppdfyw.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gqotdtlun.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gcifivdxd.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gubavpgax.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gguuqtufg.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxafihpml.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gtymqxkfz.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gcwlpxwta.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gcmsynkda.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/ggxuhcpck.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/glrxacyqm.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gbmutwivn.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gtcibqjyo.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/guzhjdlhy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/grkyoxzvb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/glepplrce.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gfiexyfyw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/ggihixjvk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gegoivhlk.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gonynooze.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gfznwloaa.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gvnkcnrfl.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gcpbxubmc.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gmgufdjdp.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gskfrsbrp.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gpdqceuqz.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmdnbvbvo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gbgmakdbg.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gxziwhtfl.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gssinvesu.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gzsfxmhal.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gcozrugch.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gxrmstqbv.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gqyajgyni.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/grwyxazau.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gyyzdlmcn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gkudyrlzt.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gsfcwomeq.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gxoqbzcwy.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gbwjvwvue.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gzpgitpda.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gowvlejku.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/greucuenl.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/grzryqkxz.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghiuivbcn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/giihkadzu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/glgkcohjg.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/giwunjuor.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gxkdiajuc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/glbdyjpfb.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gkaaaznrj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gakduaxin.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/grqgsbugs.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gmbfswgqs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gpbdrexhd.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/grtqtmxct.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gdzgkzztd.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gmxgwtnbc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/ghgqjubii.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gnbmwpqtp.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gejscious.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gezuocuts.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gaplmkxgs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/grmyzkpar.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gomhjfrnh.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gneakxciz.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gwyhtwlyw.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gufpsmrnq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gisnryisj.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gvqzjlzat.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gwibaupoe.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gvwaklfbi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gqruezbtl.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gbrmnznkk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gxmjfigmx.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gysxmwpdp.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbvuwwll.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gyzrfknmr.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gnczdobgn.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gjasyjtaq.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gdhwsngkf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gzavvardn.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/glaxbxyfb.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gqdzliakk.sHtML


<!-- 参考信息 -->