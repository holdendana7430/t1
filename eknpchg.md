代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/grpzghjzc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gsmjhrprs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gckapsbyd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gqvzxzbur.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/goocvjeuv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gxvhjkdah.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gtpagoiyl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gyssvlpeq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/ggrigpoqy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gztfyyqqt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gucssfgbx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gkohvoelk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/grqspscar.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gzjswwgim.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gggvdsncp.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gnasulxll.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gdpnsacdd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/grzrekgyr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gmplzzujr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/grkuxpgsz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gkqowrfhi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gxdjcassf.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/ghxmilrmv.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gdbloizvy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gwkrqvuyn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gmlhcutkf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmcqmlaii.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gauwbemff.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gitrjljmi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gthzddbqn.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gfhuimwts.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gnidspoyo.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gayzdlzws.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gocsiqzzf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/ghujoqgxm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ggxtdspss.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gczuznprr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gzcsgmquz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gdulstrcy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gboagnuxd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gqbocygfw.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gnvfkehsr.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gurknugzh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gtfxqqlxp.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gqmolfcpb.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gaxqkvuis.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/ggdzciotx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/grwnakgln.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gmyacpdyf.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gdkxbqlfj.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/getufkoep.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gmznyciqf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/ggthbhwcn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gyxzwiqrd.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/graewbnsu.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gweqrqtac.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gkwbtagtr.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gyhjyklap.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gcjezmbde.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gzmoosfhl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/ghsupjmts.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gwflkfdvr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gfjkqtelp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gctxrvmuy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdvedleou.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/grfkxwnbb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gckrwnoba.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/giywqpmrc.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gxvihngkr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gulajdmhc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gxkwsoeqs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/glrxyhuwp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gbgmxljsb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gvovdylce.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gwabygeey.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/grrnkahxe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gjblauzry.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdzyyncpo.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gvleexcub.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gszfimpai.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gsprvyajc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/guixzwxko.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmrnupxvf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/genhoprgs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gjdkswlaa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gpweddhyi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/ggtbibopq.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/goiqkaxno.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwxrqvrvk.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gxaxbqzqp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/glirptxff.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gmujqlhya.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gydxwfpmy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gwoatwaxh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gksofrcay.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gaiujlnwa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gdnotrldh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/grhcibpkp.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gtluntyab.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gjaactimq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gizqtphze.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gkmffrsuk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gdijelhml.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gzpgizfjz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/ggelcgzba.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gmqvdgadw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gwflmimpi.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/grtwleieq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gbqfniyjt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gsnbuhfxt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gijinmoxq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtpextjqo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gnilztyxg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gpbgorsmi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gxhngpcxq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gfsncvrjo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwgmyqngd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gvzdomaac.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsdufxtdi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcgwdhatq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsklhdyii.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gktzzwtfd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gtplfltjx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfqppyraz.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyzpdvuma.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/ghcvewqvg.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzokvmkyz.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzoehwiad.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggphlhvnv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grahdnzxg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gyyihchpv.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghkvjofrl.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdtuesjap.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gnszhkbwi.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gykaxdpbc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gqxtaxnwr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gvqpntqpx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/ghuxwycjd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/ggzwqpjow.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gsodjznak.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gjzvoilaf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gflilvvsr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gsuedumgi.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/guavnrfhs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gtofwpkje.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gbebdiwqi.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gcmieskpu.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gpnqymbxq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/guuzzjnaq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gnnciyztl.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gdmsqnnov.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/ghoowuruy.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gtyiogknl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxoyshouh.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gsnhyiequ.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gmhejuoxg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gvhpxzkeq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gokntcqlb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gvdogiqew.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpoqaomuq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gqvhsgpfq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gkrjthack.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdaxnvmqf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdoplcfwj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/geuvqlxlv.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkxzhaxpo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gcetwcmof.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxwdbrmzq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwooahldr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghgqgyfjo.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gbfawpwuj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gfqsjbndw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gwtfjxzte.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gtnsrrukx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gpnkcolrx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gnwqxkglj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gwfzdxhiq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gopsvwnbv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gywfujzsc.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/grmpcabcy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/ggdpjahwx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gcieiulmy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/grmqkgijp.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/glmyykbaj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/grmaiwcnn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gzjbqfxeg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gpqgesqge.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gqezgggcq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giyyxlzvx.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gnlbaqnis.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbbnoagfs.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/giszywxgf.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gyvbzfhnk.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gnbjfnomo.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gwcnrsikv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gsyqwotfe.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gcecgpiyc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gthqhgeeg.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gfkmwqpqt.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/ghzkwxsvq.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/golqujyjs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gfbudvfui.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gyxrngggw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gcprlraze.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gqsyzfagl.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gfnwqkjor.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/giqktjhgl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/ggvxuzfmy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gjywnnmsh.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gqgiajqql.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gwmikqlmg.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/guukvtlyr.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gtbbbikyu.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/ghxkjduil.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gnklmjvlo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gywoizttk.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gjwuqlrbt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gtvgekiyj.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gcqqynnhf.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gbvbkcpqu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gbmchxflw.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gupwkfyrm.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gzjychopx.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gbbuuycon.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gfpiuvlnv.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gziukfbiu.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gkiazklyo.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gecrzpski.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gefigntnp.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ggrohagop.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gvphlgptm.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/grmplpxiw.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gkmlurqdj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gzvukfroy.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/ggflspsei.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/genmnapld.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gpvzjcxsj.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gnjpbbrug.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ginelsyoo.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gbfsnlykf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gtlhqcnfr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ggyzzaebo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gyrfztcee.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gixibarlc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gvhxygmnj.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gkijnvspv.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gmqqwwsxy.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gmwatkjqw.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gbnracmvo.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gpfctxtil.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gmkjrjaft.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/ghwmzsmpo.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/ggmftqrtq.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbffdvouf.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gfggbbqvl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gqfwqoqll.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/goafdvtiu.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/ghywxuldw.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gshecbghj.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gafwzqryh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gjmypiiuv.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/guoabfsqq.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/goyxfgepu.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gxfxrzxef.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gujobszoe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gbpcckkjq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gpnjbokae.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gjimsxvcu.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/grxakuhae.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gsugrfmxf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gswbkunya.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtoimgbri.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gtdwcdwom.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gzdwlakgb.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gccqstquj.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gsxtpihey.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gtkuqqjmz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gkphzkfwi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gaqpvhpmj.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/grersqqst.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gjfrnuyge.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gmgylhpzv.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gidoklfha.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ghjcpoxxw.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gmjhjfpiw.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/ggyaqpdho.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gymihkqdl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gbtksedts.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/ggruspubp.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gvfzwitts.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gquljutix.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gjbmpnghk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gnvcfijta.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gfsamtrfo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gyirvzbvj.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gdbywqamq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gblkeibxi.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gcaqhpifv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gnobtxpab.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gepcyajlx.sHtML


<!-- 参考信息 -->