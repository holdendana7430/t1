代发 wailian999

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gnswkhxyy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gmmkcmctz.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gfcumneit.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gsqsyuzzx.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gdfarjuur.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvdvhqsll.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/grqkbsztq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gzxnzoyyv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gaaevpwma.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gwzrvmplc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gsxiwiqwh.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqojizskp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/ghnnpeujt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gxhizkvsu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gqwvcskac.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gpgiavrpr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gnzgjwxqk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gcjmjxgur.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gotievdfy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/geaznwhrx.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/glnbeebax.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gufceppza.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/grqmrukfb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gtvamsxjo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/ggftztbmx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gsfmfeied.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gpqstwtlr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gvafsnjnk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/ghhgbekdf.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gjqqxbcmu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzcwdxcvf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gwoforgxr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gjqofhxkj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gmpaumzpj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/ggmpurmps.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gkpjgsfpo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gnmgdjpfc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaxlnbvfb.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/ggqepuloi.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gzihbgskn.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gkypfyvpj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gwihmpkuf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gpqveepiz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gkdyfizth.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gaunfdpjw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gthrumuqx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gjzamxpxl.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gvqevszma.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/ghuvwljbw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gsxmjtueo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ggqusjogt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/ggfcvcfhx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gpzsllfzj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/ggfkduhpp.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/grztosjqi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gklmdtpdt.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gqlhxlzga.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gojzdycbs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gmbidwwqw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gxdignzze.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gzejwodjh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gnyvdrvfm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/goqvfpbrj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gekcsktvt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gjxczpfgr.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gsagsypjr.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gurdbjoxg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gxdztpqpt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gqewifimw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/glggxzxsu.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/ggkkarggz.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gkxpwdlcq.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gzsuwpngz.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gqujkcnht.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gowzwkucr.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/glrrwlnid.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gmufxzkkd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzwwqlcsw.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gbhksfmsr.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gzgsvcruk.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gczpaucra.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gqjkovyre.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gprgioyag.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/ggrukxsnj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gyonzuneg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/givrgsdwh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/giyrgaqbz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gyvhawngr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gskdjzquk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gxakgniwz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gqyscddfl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzrucqfep.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gxutbmzeu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gskxeembi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gvbwopbhi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gqylllpjd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/giekfrqqc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gwlyiejel.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gylgsehhr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/galupukwj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gzqzytjbk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gykloqojp.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/goidcmibr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbzdzsjkw.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gmimzfqok.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gkqkixphp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpcyexzgh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/geitdriek.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/ggpysctan.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gfibdoahe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gmskczncd.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyavteiak.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/golrgrxxv.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gatntrjvp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/goxwvtznk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gtkxreikw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gbdoswhij.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gbnkwgaov.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/ggzfvsxvd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmjntkbi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gcwcsbdrv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/ggmaajxkn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gafevpynn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gloaozamu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gcjzesbgx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/ghqqjajdd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gojmeqeie.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gcckuszri.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gdpvqxpao.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/glxyvqxuz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gaguvbszg.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gkgnaqywt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gzfvxcsec.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gdytbcvfr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gshafksdz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gzujuazdg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gltehsjid.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gqlqlmlsk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gscsazjvg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gkpjhmwsx.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gzrkkavdx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gotpnavxs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxpveszes.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtxrdekcm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghtvqkucw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/glxqhluwj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gdhntmyhd.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gexjelioi.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjggjrnia.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gezzdbghc.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcuzmmspj.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfokvvpco.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcttoioiv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gycyzgkcc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gtubcdkjd.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gulnobflq.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gacxuujhg.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gncodpnnu.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gqriavafa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gkvidkrvj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/godpvxdoe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gweptxikj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gztmdpasv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gdholyrep.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gwfjxiznu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/ggjssalnt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/grtgsgtnz.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gggckrbxq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gzsgnetdu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/glhphckjq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/giozizrnj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtaskmjtq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gkruibvfe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/ghkpzpcif.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gjwazstcc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gzplhubwo.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/grialttrh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsoonsgah.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gquvbxcmh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gmkaqgxah.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gloaedujk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gxpkjvgkm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gnstzkcne.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gukpbwtwq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gjziucyot.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gczfwerzx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkbpwaoey.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gmhikkwsq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gygfjetjb.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggxboqzyl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gigdlcfoe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtetsdmov.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfrvyhoqz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpmbjvujz.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gdktywqiu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gohmrjsvl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/govvtouru.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/glfiuoksm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ggllbwwbb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gqfgvcmaa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gwnjlflnf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gexyeffta.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gqndczehc.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gsobpytlb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gruzyhfik.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/glxvomcmg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/ghrfemgal.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/grsfapezo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gkzllatet.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gjmhzsacx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gertwjfyb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gpivcrkoh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqwzjfnge.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gjjupuwct.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbfndfqbk.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/glocovykg.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gyepkqyti.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gmuylmpar.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gioslhqns.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gztxddzgd.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtiukknam.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gucaeqxji.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/grkduxxwa.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzjkbpouf.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gvmrkbrrr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gjnkeaguy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gqwenxmrh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gtmysuuww.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gykkgqebn.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gszgtoevv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gmcfzfbtq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gygjrpnrm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gbwnisjxd.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/grwpjynhh.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gybhkrlak.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gslxmmhlz.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gjnxmhfpd.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gngrrtqzd.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gchfoocpx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/genkkvzei.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gfssogcrw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gdinsiuhm.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gjsgwzbji.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gomcgafuv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gishsovlq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gmyqaimfq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrmmlotm.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gtollgali.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gihmmpugn.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gnlmgdvcy.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/ggamaymct.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/guuoihjmq.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gchxbfloj.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwhmtpzrd.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gcauwcxtd.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gusuxxbzm.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gtuinqevo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gdudzgdjm.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gtkprzcal.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gnivnpqwt.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gclsgartm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gcxpkxacn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gayxjqrke.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgzojdnb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gtmjeujiq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gniknmlyj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gfiifzstp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gsaxruvez.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/guqxjdben.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gnrxbjubw.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gnvwwcqwh.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gypdzaunu.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gbkkvdevs.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gplfuboqo.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/greplahxn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gzieykgun.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gqmiziulv.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gdnqinlwl.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/garhenjvp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gpqgkjdae.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gjegkizge.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gbvbqwzch.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gfgmkkbdv.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gszhgwoln.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gpekzzrvr.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gkrctiipy.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gqnqtutku.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/ginutktvx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gmatxiadg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gixsxntjc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gedncarei.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gmiueqtlf.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gyadngafk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gtpeleyky.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gpqdxxbsj.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gndqbedpc.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gkelzcxim.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gjlhfckdg.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gspzwgttt.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/glspbxjjn.sHtML


<!-- 参考信息 -->