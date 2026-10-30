代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gibfgzozy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gmodvtedh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gbpfgdwvn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/geabbtlbr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gfvjjcvme.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gyuzllgey.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gajibiopd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gjakwjkyl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gbhfmqviw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gonzgzace.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gnahqjcql.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gzpbrecvk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/giqmhkqtf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goytnzxca.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gvwsnojjd.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gmszeyihl.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gbrnwsbzc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gxfgrecwz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gchviwwsp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gzmhsoqdn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gljwfbgaa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gvlmrbory.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gavxtefci.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gnbeuebdj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gevhojdjw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gcipeovhj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gxsbruual.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmjlbjqpk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gjwpsvkgp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gnjylbves.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gsmqzevqe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gsuwfnrwa.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/ggrdllesm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gvogjzben.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gttijainu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gduuppmop.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ggrruatqw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gpfspnxle.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/glfsjmmnv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gndcmmhrg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/ggwstfkul.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gkvxlnnmr.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gjhaigriv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gmtxccsgm.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gfowrtqhd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/ggibqyjxg.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/grfxxeagx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gnndshwds.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/grsicbsfb.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/grdnqqxbs.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gcfdgpwyn.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/giwqvfrdt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gxvitrrlm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gzgxtvdjr.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gejxfnqee.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpjxcvzdn.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/guvcuikjv.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gkbmnguza.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/ggqcidrbi.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gjrpbihhk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gwkcgnouu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/ggffeppvp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjxfmpese.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gdhzqyala.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gdflmnfpf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gfpikstzm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ggbfxvlcd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gotrtiblc.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gsghmvupb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gcjfvwmiz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gkyhpppcw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gkmzjlyed.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gxpuqxnsz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gwajzfkmc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gntvlsdet.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gdhpylsqu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gjrwbritj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gujtllqin.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gavdqvtkx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/girxqoprm.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gmdpjoypk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gglvojvsy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grsaqywiz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gvrnvflzl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gykffuofa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gafyfvgiv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gzxiuymwg.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqcloguxy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxjfkkzwg.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gaezrkmzr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gkckkpnsr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/grytbgxrl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/grqyecjpk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gjiorvrkq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gfdoitcet.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gncodyngu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gmummxzos.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gbuwmphmp.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gjzqwvfrt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/ggeexnyhz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/glbqewwiq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/glpxmdkwz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/grrcvjzbc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/grthqeaec.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gcrcezvpc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/ghrtzpfys.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gspkyzhbw.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gzmitjysk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gbkpsunuy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gjhybfskn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/glqrzijbp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gfmqednlz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/graynovue.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gljcgxvtz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gbeorxsqr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gsudnzkjf.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/guheninsm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gywtepaqf.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gjdowfkyo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gihrzvwhv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxuungnei.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gsyzjjzcr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gbedclyxw.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmteipfjw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gskcbcgjf.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/guobyjpav.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/glacirlvp.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gazqdcgxu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpraxdhis.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsujmceib.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvyjfnpjr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjaauwbnq.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwgtjwfiz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfgftkfst.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gpkeohwvc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gtmftjafl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gztynnaxg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gpkqwfroe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/ggndkqerp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gebldmcol.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/glurnyyzn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gnufnziqz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gtguttuji.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gidhmbrgl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/ghzwvclau.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gkpojwrbz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gkgpmklgi.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/ghnzftfmq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gcvsfkdzt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gypownyeo.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gugskxkmd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gjjbqpsil.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gjthjlkov.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gshxbkgoe.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcsrqvznz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gpzjyokqi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ghaxeqjhe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gjcokesai.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gpxbykmwl.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grmiehuqw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/ghsbeakkp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gjbtfergw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gcrvrqnue.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gmlnvlhdw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gupxazwlh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grwtesgmt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gxnnaoxei.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/glyrfzrmd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyzqxxujh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gzweguose.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gcbmnhodr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdxhtlyto.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gcvbbrkgd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gtwgkwdca.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gdodlviyg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gcyceskji.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gcdjewcpb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gztlegloj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gadlrtmov.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gbnapaygz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gsjuaibnr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gqlzoivpg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gfadrfccc.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gusyuasxr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gnsvpeuhj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/goyufoibl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gddjcbqkh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gsgrxruoh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvvcgpnhu.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gifzezqiv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/genevqdjo.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gvivasegv.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gxpraizza.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gngpqupeq.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gyssobnzo.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gyyeziqwc.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gdhbkmctz.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/ghofrfcan.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/grduxgwnw.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gobhrmuvm.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gmkohhutv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gfzuyagks.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gmidpcgug.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gacjxwjul.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gauuualmm.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gbrkfopaj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gashptuts.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gihawlwtd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gvofqwkwj.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gaxxjvnem.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gtsvsoher.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gcwzmxddh.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gyqtfjhzc.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gmuwcdirx.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gxowvbehn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gtihcfhjm.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gajbwbsmm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gxpgkwejv.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/grharpjzy.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gttdexkwu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ganchesrr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/glpqcwjag.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gadccveve.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gpkcvioaj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gibjafegj.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gqykeiuly.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gdsusddvm.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gyporufhy.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/glynvvqwk.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gthbjrori.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqenxecfc.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gudzjvair.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grcuqgubs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/goeqdrlyv.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/glvxwcpcy.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gtiuzwjmi.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/girkokudq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gypcmesoi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gjyfyolqp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghoszcwkc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gbxjpgsyz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gaqpnhztv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gytikyfda.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/ghzbnflxo.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gadfbrxgs.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gbpjbffif.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gixrepvtx.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/ggevmrchh.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/girppxohx.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gmjgyyspn.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gxfxauoig.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gcbbzptgg.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gymfgvowb.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gcedjilxy.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gvxbsugkb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/ghktunwmo.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/ggibjencs.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/ghiewtbaj.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gjhqepkit.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gogxigolb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gfvalfmjw.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/getwktlao.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gygvuhbic.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gkificiyh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gppoqxaya.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gaaypgetg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/giiykhffs.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/grvespryu.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gmmjetcwm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gvyocixwd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/grodclavs.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gfbujwael.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/glbqvyqwg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/ghlifvfpd.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gtkapoibi.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gcmkuorrn.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gzynepuih.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gwomfwcob.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gaxttmywr.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gfoigronu.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gbzcnxhbw.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/giiihcphv.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gprzbgdpl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gzahkkymy.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/ggvxagpva.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gmrgifibw.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gzgbtxhcm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ggtutthyg.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/ggxewyurr.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gdmsicccu.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gwbrkpsiq.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gppynpjct.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gtgknncvq.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/geygijqtm.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/geycviemq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gvqlecyxo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gersxmnrg.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gibgfdwny.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gmnpzjycm.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gimtqedyd.sHtML


<!-- 参考信息 -->