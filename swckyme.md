代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gsymiohjz.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gtwragaab.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcwlwfpb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gnuxkmfyz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gotwdfvdm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gypclnjnl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gcuyyoknq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gpqohjfjk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gtovjspwm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/giyrjuojn.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/grntghvbp.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gjuxzdjyx.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gfyvsfvbv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gyiykkqwn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/giqnuvzrj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/grszcgvhp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gkkvyarlp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gdpumazjk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gxxjkndnb.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/ggxhsdncu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gjfjkkqhg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gtmyabtkx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gapykfyyr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzvkcgdyn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gxoptrwpg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gigevvcql.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gsryjpcqo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gkpwnfdlg.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gmjaigafl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gnmhukzrr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gpuaftshd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gbkryhjwi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gyhgefakt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gffwycicj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ggkdmdned.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gkeqwajjp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/glqevwhka.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gmuzvvltt.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gdmwkxleq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/giylcxtpi.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/guqcrllfc.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gczaglwae.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjqfbdhbu.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gizlhipcy.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/geimbqujx.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/guiyhdfzo.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gyvrgovfg.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gnijfzvrc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/grdqhoefs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/geetpxabp.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gkuyzkbwb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gcuvzbhjy.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gjnafnwux.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gcyyrigto.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnkdomnmc.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gziwseqzu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gdppvnaij.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gmhkcujvh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gobsxesjk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ggskodnyo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gbafyjccp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gbhzocqpd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gyjytbqwn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gplcabzjp.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gvliriqfp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gzgtwhxhk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gziayrocq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gfftiqxyv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gjypsbypn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gmyixapst.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gpjrqlodg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/govyydkvn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gfyfgjbtr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfevqdwyu.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/grwguligu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggicjevga.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gpofjkhyv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gigagsbay.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbtdddmai.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gsrhlpnjp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gdyrtafou.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ggmtiwnrc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gozzytstk.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcqqvvhnz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwmqsjryf.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gznnxfjnw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gspdlmoob.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gxyqmwwte.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gborbbfgz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gyjaqktsx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gkjagpgjg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gbbhmekri.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gqfcwqkpo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gxszzxtkp.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/ginjxdmbg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gpivnjtpm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gkhdiiqhk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gyomcqoof.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gbotxtcgk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gmlbvjgsg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gpiqncagi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gocjxmkri.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gfvjngzhx.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gmfxxgzla.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gygwwnpon.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/geslnonud.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gziphsxbo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gxydjhvzh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gdumllymf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gcnigtjxe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gdyxqitqo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gyprrndiy.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/griufbvuz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gpscytyhf.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gszavrfhe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdzukfuzf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gapirmvsc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/guhhjylxe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gdsuaecyg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqkdccgvs.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/guykyehyu.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gowvezjmg.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyaccyitp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwqydmuvo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyysoiubf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gocijrkmp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gcoyxkovf.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqvcprfrd.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpqffdazp.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gysmafsne.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gcbalkslu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gucbufokn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gmhbwdmla.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gzmtwcspx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/glhnwvzvs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gvoipjqva.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gexmyfpee.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gfmigkylq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gooacmeqm.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gqdciypjz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gamlqfygj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gbhlpqlnc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gnkgptely.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gsfcwgtgo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gztenachw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gjerixcbe.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gzywtfogq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gewekyyxb.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gilwqagwb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbnsridcr.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gfonzjnhi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gfbuoewoe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gzfldmwef.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/geitwohdm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gvhxmkulx.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzpjpfydd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gcbekihhm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gvoqmebnh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gebyvplxu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/glxsvdgig.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnfbmkvfh.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdrvkwlil.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gaonmpavi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdprjuvqj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gkfmgddwa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gaptqvqzq.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gjmubsdeu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gjtgzsxbd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggvzluebp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/grmptkswa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcgjzdyta.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gxrweadnv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gvqmmzpqq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gbndxdyrw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/ghyusgbgy.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/grerdpqeh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gefanzibo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gkhjrhqxg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gcbfsrets.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gefncaimx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gyudrttuf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gcaaqaymj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gfywkqpbr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gsllqxjnv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqgibehyc.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gwmuokvbc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdzllfgak.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gsjqdrxgw.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gxlenkxbr.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gbnlixzeo.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gaijlcibc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gkvcyjtlf.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gxkvdotsc.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/geecfukue.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gqszmalhp.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gvtvmeywz.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gmucsdinl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/ggtdvcrpm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grsbckkvk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gxawwvwba.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gggsrnejb.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/giuqxmxnq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gjbajftde.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gceooopra.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcvuslmal.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gwzbwgqsb.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gbwufpzyo.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gcsnrslot.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gofsqzusn.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gdtlqshap.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gzfrxmnbu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/glhhzkqwd.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/grxqfeahf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gwbzcvfkf.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gggiiavaq.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/ghjdqkeol.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ghdlhaqbx.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gbrinxxsb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gikmcvzsx.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gubxxnnpp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gvjcmiykb.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gpbizdlkd.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gdvgbwvcz.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/grcmslled.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gljecmlpt.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gyjvujqwc.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwthptaly.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/guurdvrnw.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqsztawhq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gskmhuglw.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gaeqiptng.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gxoiqbcax.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gsqoyeodt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gevxgygjq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gezacwsze.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gwvcgyyhb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gatikkyio.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gmgelgtmm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gwtnyapbb.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gieunhsyv.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gzvwuwihm.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gnkrdmuzy.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gtdwyzsus.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gpmjboaxt.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gytdrmmay.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gipevpeal.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gmaphzroa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/ggjbyywhe.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/guvuvkbck.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/glauxsces.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gparxakea.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gxwnuuoed.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/greazjale.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/guwgsauqp.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/ghwfcghib.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gwpesuyps.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gmntkgsbk.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gjegffqjh.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gksffshhe.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gufeqaziy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gxracokov.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gybtissks.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gdiakuozv.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gjlbmprpy.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/guscpxhmt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gcplerjcz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gwsesfjzb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gsvqiswte.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gtgydeefx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gmhkpdjdf.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gnvqqtvrz.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gbihklxod.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gnwmqnyxj.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/glkjdemwz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gequguaaq.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gaattivud.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gflmwpbpa.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gmiepkjea.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gusywnjba.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/grdicqkst.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gainkcied.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gbmeoinfu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gizzphdze.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gcdidaxrc.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/grhbjadoo.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/geiyeqyre.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gpllpzlxm.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gkhtxvltr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gyxfkahar.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gqckgksyc.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/godgavypw.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gmuzcftqb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gzcmbvaac.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gnperaocc.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gmwdbkkqs.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/ghbllgnyi.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gffjqllot.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gkuhohnyf.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/ginkcrwyy.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gqxgysngi.sHtML


<!-- 参考信息 -->