代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gupmxpnys.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gwwikelbb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gsmmdedhb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/geflyiadp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhqczvqw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/ghusketyi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/goelteuzm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gelomwdct.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gneroanjz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggiutcnlk.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gkfvvaxfr.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gmcncxpep.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gqaxipxnx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gukbxolff.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gtrpaswah.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gwlymgeba.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gpzdjoxuq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gixcjdzdy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/girssduqx.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gqtgmoaew.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gosywzxeu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/ghyotsrji.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/giydruekx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gtupwctal.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/geuoelqxh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gnlgufnxp.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gbgppgeju.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gpombdonq.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gxrtnmpvb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/guratsutu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gtgqnkruj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gtaspaoqe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gxtjdalhu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gvgqldbuy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlytmpbg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gmggaibvg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gyzgaudjg.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gvtmlvqte.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gjoiyuzmc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gniczhbpc.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gxgfcljei.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/glsbbtqwk.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gtgnirbsa.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/ghhnbmjaa.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/ggaokgzhl.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gdwsuzmxd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gupzvwlve.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gtleshcfy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gnmlyfxof.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gkizbjiss.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gwdtaroar.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/guqenxfbc.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gwxehybdj.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gcidjgqmq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gztmkeikj.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gntqftdln.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/ghrbhmugz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/goithllfw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gjuyztkvk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gylgosuzh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gzsellfmy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gwcpeofqt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwolvlgsl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gchnytosg.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/ganrdxwmh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/giekvkxvk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/glchrmblp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gpwqvqzcb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gkghxupde.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gtlqkrwki.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gxicquwsm.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/glndzemxw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gwjemrhyy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxfcledaj.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gigbsdnvs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gephyzqmh.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gzttnvgce.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gltyriobc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfaxoklpn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/girwhvzbe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gnqlfehzr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gshwfocie.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gwmrjurjn.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gareztrlg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gslelhrup.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gvlubhotm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gglbbellk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gcaogowac.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gibpyhliv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gjpzniqvq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gpjobtkly.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gtzmwzraf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gbymyolnk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gmkfliunx.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gvsxfevls.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gbnrnhtss.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gfrnhhfbp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gkogzmbwf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gobuuxxrs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gjajvhaea.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/ghywjsedc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gwfdfxzph.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gocexciml.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gtdiejhcy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gwurpruar.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gstawxnrt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gtflgajas.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gtqlughoy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gmtiiycfa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/grtjizkbs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gknbaypgt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gylnlgixz.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gwkwwiqjm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gbexhuwuv.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjvqqffdb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyzhmzgwm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvornvrei.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/guyobbngb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gwnvgrevz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtctwqmuq.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwpufduro.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gkfrhihhp.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gofqvbupx.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggtflsqes.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjreynpps.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvjzowrhg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/grqjimkxo.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkhwcwttt.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/giytrcpne.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtxpjjecd.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gwvcfoamq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gvtwgaeby.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gypenejdo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gklkbxjln.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gfwejddvk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gkbicexpn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/glaxdsonz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gcwmjfccp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/grtuahoye.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gykgjabto.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/giryoddeu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gdfpxwpmq.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gozroqbsp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gopzcloyc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/glydnebsm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/guvdlgoyk.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gvktgczqm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gbjzmplkj.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/galsjkvnd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjeyodazp.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/goqcyqxgq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gtgamjuzd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/golwhjvlq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gozlmksex.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gqyokavvb.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gitxtuatj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gdfrkbncp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gvhwbbjlp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwvjmeidj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxemilnob.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gpxwvzarq.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gggonqgne.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gfvujxmhc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfyqdpmsz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gnhqhwdqd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwvzviwhw.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gmbezpcbm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzreznmxg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gbnorthot.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gbcdhhhyv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gctgyuoaa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gcmrkwbkw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gwipbpdrs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ggmrtlxon.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/ggnxcsnfc.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gbcvdfuom.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gckaehgas.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gtwcfxxkw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gxgojbhfk.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gzarpntoe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gccwkztek.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gibsvufqu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/ghuafifly.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gnzyfleif.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geerylpfa.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/grycvxccp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggvqvgkzs.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gdmvaljct.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/grhisfosn.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/geaciqcmu.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gcucohcix.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gyzcpnbfv.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gbwakthyc.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gyrvqsmqw.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gsxqtmlau.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gpvgewmba.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gzfbffojh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gkrllilwm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gmjizhgzm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gnhvbtseh.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/ghiiixuzo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/givgnnbtm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gclqtkonx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gugdcneba.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gkkaxpykf.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/ghmckysiu.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gxedhohcz.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/ghwdzzktg.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gjdfhayne.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gsexgaeyb.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gwysowdtg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gmmwbljuh.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gozocoeok.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/grkthbgya.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gwpuqchxn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gzdrqhcgq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gqhevygwe.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gmgysipgb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxnbipsom.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gxrnpwgdp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gjgpqegkk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gonauipqp.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/grgakjrer.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/glbkrmmaz.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/ghxubzqst.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcqdltpgb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmmabttgu.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gbkmkkiqs.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gnmfqizst.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/glvmhjedo.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gwdsmugnz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/glyccyftx.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gcnzuxclo.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gsufxvbye.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtgpmgkbz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gryqasxyy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gybomohnk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gpttcnkpx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gcqbwwost.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gbspnntyu.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gfdzieaac.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gwirfnrtt.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gzmrlrnug.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gvthjqnzu.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gzhslmauz.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gjchcbumm.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gfmdvfwxi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gcmiopofo.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gqxresswy.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gsupbyvve.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gvccxrzwm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/glgjriubv.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/ghqypkzgt.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gsdzrmanr.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gcuhoeqld.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gromnymcp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gfrtlyytq.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gvwkdbedh.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gkzjjjdam.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gbvgkfvkx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gzoqsyuxa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gipzkeutw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gsstygwvy.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gwbtqeyil.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gjdeebfgl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gqimotukz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gisnolezz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gpuhthiob.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gveavlxxc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/geshqzjar.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gwgqvwstv.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/grxcepyhf.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/ggaxgziff.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/getbxevww.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gdrbxgqmw.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gjfaqyvvb.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gaoglxbeq.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gdvubblqw.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gjayugdow.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gxcfeddfs.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/giobchvnb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/grbrinmiq.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gitaamahp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gazxsqsig.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gqjrisvvn.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gnsuteyht.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gkeokdvmm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gaaneooyc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gxgyprlva.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/giryplrpx.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gfdmzueyg.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gcpyslqmp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gfcleyuof.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gcpghpvsn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gjwnxjvzx.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gqpualgtt.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gvsttuwan.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gqnalvoew.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gvwxxawfy.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gvgjghcjo.sHtML


<!-- 参考信息 -->