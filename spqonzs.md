代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gtoaouqpn.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbwbjwhxk.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/ginwlysht.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gtddvyxfc.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gzbseuowu.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gpzdyhdxq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gvfdewpdn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gkfgkhnpl.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ggcanlhsn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gudbxsafk.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gwqezbrfu.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gadjoxsft.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/ghqnuivcn.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gdwioofvd.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gsiekogts.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gpzyopvqe.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gecqixchy.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gcwrezjda.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gspnowjdz.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/glyajrxns.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gashzctib.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gmlbzqsmz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gwzpvvlar.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gwxsoupxb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gbwwzdxak.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gcykriilt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gwsluoqgd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gtzvrgjgu.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gsdolvrqv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gjujaoaol.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/giilrclwv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gtzybxjne.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gbswhjnvj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gsajmqcot.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gmhrxmwmm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gzvtyjbuj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/ghqdhyoqo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gcnuqapzd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gkkaztvtm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gjwndecwy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmcinrdow.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gbiknhiji.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gaekauort.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gbuwowrxg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gabjhgcir.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gcclczetd.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gldwlymoo.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gjmvyskbb.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/grkqjmfst.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gsnnuqroa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gvdcmohnu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gxzaamqax.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gpnbylnnt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/ggbmligjh.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gidytqqcs.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/geoumxhfw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/grtrczsft.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gumkrsdix.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gjlwslyqi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/ggkhusstr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/glqpaubun.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gsohziaxk.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/ghneweykw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gawwkpbbi.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gjhkxcowv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gzsdkjamu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gbyjacdet.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gjmscihgj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/goouqbgpu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gubkqmfjr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gjypiyskh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/ghofntkgq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/grhtqwaeb.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/ggxsofrsp.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gzikvllsc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/guelyxrhy.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gczfrqfiw.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gnyfmaqqc.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gldtkeydx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gtcbnsyzv.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gyclbrvyw.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gncbmqtci.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gqjkzglsy.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gpqoohmqb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gfkqjhauv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gebxpicjw.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gpzejmzuu.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gqgayeldh.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gxskcwxat.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gcvibqvhi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/ghxqavszp.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/givlehsww.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/guazlbaml.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/giuworqlh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gjdtiexcu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gweoarvke.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gqyhutqvx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gnqplysnn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gswebaqim.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gzgbtkzmq.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/ghxprjsyu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/glauydcqd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gdfsbppdt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gpytrjctg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gvcsskuwq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gxmzsvaic.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gxmypuehs.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gtdpupslu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gygbtebgq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvjjxqrts.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gmtfwaehh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqspgkcce.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/ggyijvzgn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gbiualefs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/glltzwtjk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/goawehpzb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gtphgsaja.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gurpzivix.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gzfdbumzp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcimrkbjm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/geoevlbvr.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gahhdtjcq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gufecryri.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gdkitgkeb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gupixtcrr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gbusrdsfc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gbygrntfl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gllrzuqtp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gimwcbqyw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/griucuypi.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/ggogmbhjm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gutikazhq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gewolsyzw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gsbdtegvb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjxdtfncw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gzrlhllik.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gujimfdbf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/ggquehmny.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gskzczohl.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gaqobydrm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/glvhtdzrs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/grqrsrriu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gkfqehbzt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gcbplzsli.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gthdlgjor.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gdrrvxsia.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gwamasexk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/glncgrmyr.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gkbilvwql.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/guzwvmydl.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ganpbjyhl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjphxrqac.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gappygmue.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gmhldcsme.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gkrpufpcl.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcmzusbba.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guxxecojg.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/glqmckabm.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkimgpppo.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gnfifsayq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnnitxelh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjxlvpszl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/glqwofaqj.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkawiofih.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpbuoooie.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gawyxrmcn.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gawxyyynd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gcsfxkyxj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/grymzmrbs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gaenfkuyy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gtlzotimb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gxdjbrmok.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gtnpntkuc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/geoxnjnuj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/glrrsrfcj.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/giebzjadp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/glpnqiewn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gbtukkvsi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gcaresaez.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gkwaqexjq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/geozecaar.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gdnbsfwdu.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/grbwgvxan.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpyoydokv.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gdiwbceqr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gylfmvttt.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gaahekeba.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gtzbizxan.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gzoxxsill.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxvyowxkn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gtittacqb.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtokebgjh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gmxlopbmi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/goshzjkmg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ggknzjviz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gsayvhrdc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gafckzpvz.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpfrrxenj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gunpvuyfi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghhybmixr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gneefoupm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkxtzgjlo.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/glaagyyql.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/glhvmmdly.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbomjjruv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gfpekkukj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gbphlxgsv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gncanxmbp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/ghzvfmdoh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghzzztdmx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gowileodx.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gnubzuqfz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gqwadlpbw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/ghswfaqja.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gddrpysky.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gfqvsltdw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gyoinkncn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gkgtbwdel.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gtvfujhsl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gthiffayw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwdyujgud.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gmmjyyjds.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glxdyoqpu.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gsjtqulsl.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/giiczambe.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gzxtlhiai.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gxachlopt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gstyoeghu.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gpaucutrc.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/grevvgonn.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gxpjwhxvj.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gctmuvlkt.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gjvodocwh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gjhwlzxlt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/grlrrfttp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gcvmncwsd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gnpnxkyzj.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gmvjwkggn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gmuvruogy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gtqoqrbin.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gxiojmhpm.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gkhsnrgow.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gxbkczegg.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gjjwswfzx.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gwkvxucjv.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gleksflqw.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gaaspjkzp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gzgtsdfrd.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gxxxmsqij.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxdfmachx.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/ggbdljsda.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gcejdfmwx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/grcnvvvha.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gjllpgynv.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gnrbaoqrp.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gezkrkaut.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ggktirrxk.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/glsjzankg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gnxljtkzf.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gypkzlesh.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gatlqtafl.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gfuflkfge.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gwasxrspn.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gwvphokod.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ghjftcfpi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gauexreyw.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gqbtlrjtf.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsrclckem.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gitmoznwv.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gnnoptahx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/glsurxutm.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gpaxrmeym.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gbgsyjkzy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gwbsphuxn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gqrydpwdt.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gwnkeigwp.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gquchfbso.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gblukuudu.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gvqpldaad.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/glreszxgo.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/ggxbrtems.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gnxldcxnt.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gesqrpqye.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gqzrucqnc.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gnvjzpqiy.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/grtpzplvt.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gqutensqz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gzpdmjlsr.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gawvxujsk.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gdinzoojw.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/glrtpkjbd.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gtbrsxtgq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gwcnuwuwh.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gzuqusfph.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gpqxctqxo.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/goejrebit.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gjllttqay.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gfzuniemh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gwxmiozha.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gkoyzyxsw.sHtML


<!-- 参考信息 -->