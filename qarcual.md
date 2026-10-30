代发 wailian999

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gevncbawy.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gnozquyih.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gjtkddpvf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gkmafggcy.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gaxwplnrs.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gxvfmhile.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gmcxyrdao.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/grmxboeum.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gkvtlrhvd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gddutdnrv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gsejgxxuy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gtfvswyfo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/goedcphti.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gsznertqh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gyigjehhe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/ggqhdvfqb.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gjfdkhftk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gyehbvroh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/glckwmdtl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gchvzxilr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gonnpadue.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gpxzmxixg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/ghstwplhx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gugsepdxe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gosflzkgp.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gdvqgtfkx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/grquufypl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/genxonbmx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gadlqlymq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gthlthuir.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gkutpgrct.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gttkjnqab.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gwljjltgn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gxdhhwevz.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/glczsbdxa.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gdiwtfsmm.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gnelplmmh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gvolhbivs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/getbsfyyt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gqvsuoemj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gppiltfsx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gozlaztmc.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gvoymxesq.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gxsegplom.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gkllfmhnc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gtgsjstmd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gmwbrlawy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gdjgnakxh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gzlxjvxuc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gdzkwortd.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gukhtyvgu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gjrqjsnpp.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gfvahrklz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/glcpprmbr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gjpffsaah.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/glsdhcbuz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gmaihfsgs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ghfhkwkcw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gyzpkxzny.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gexhvszhj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/ghhxhomoc.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gzgfxgsnz.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gqychvwiu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gfhofnunc.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gosrqooue.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/geiksvoeq.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gkzprrjby.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gmaigcyou.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gbppaagru.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gqofiyqxi.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gyoeojqnw.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gilialnpr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gdmxmkqac.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gpdcslyzf.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gvyxkfble.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gwknrfdwr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/goqmagici.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gdrhrytxn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gdxizlrmk.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gpossimji.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/grhkadnuj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gnlypwcje.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/guzffnlux.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gtiphbwjv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwxbhkvtd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gsxrgawpq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gejonsdwk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gdvjsalxd.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gbndnrwah.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gylttfxzy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gsqornbog.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/glyscsrim.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwyuapkub.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gpiffxlsc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/grjqaceew.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gmenjvcqh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gqonfzqso.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwzffoast.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gqelkajiv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmhfvhbnc.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gnuuopxaf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gyuqamqpw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnmdwmgxx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gfwoaawjr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gpuvcgxeg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gnuqlvwod.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gsksycnzy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghbsawfrs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggnqqmmql.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gmblvzrhx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gxqztmwwd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/ghoujyznp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxtbcfbto.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/ginldslsi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gilxflxhq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gsjnlojfc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gwojivqmr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gvonospaq.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gihrfplnt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gtlxbbqhd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gbipglpqi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gkuzkwypo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gnedxzbxq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/galbstyvh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/ghekuvgxf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gztpomsnw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gcoabkfui.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gefwmikky.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gcuzxehyl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gajbqkcbs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gscxulmru.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gjabxgefs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gbtswzemc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gvbuajvng.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gtboburtu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gnlbgrhag.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gbxtvqayo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gzxzysbwb.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gsuiihdou.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvgfigyy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gklltirqo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gagkzjgsx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gpfnhevyz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gboxqrxfy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggaszimso.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gehprybrh.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwbahtxxk.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gmouiejup.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grutefonk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxdnbrzmb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gvidlalyk.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcgnyrfmf.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/glmypevia.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpdyifizm.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/ghzkanjtu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gkdpjzlnq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gxxljhwoo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gizpvuvhp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gfvxxhrnv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/glycwmtdl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gqedeidid.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gbrmjbvnx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gnnwuahbb.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gwhqrujmh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/glzxdkmma.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gjvwnqfkc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gdvzkkyep.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gczsjuaej.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gyueanruq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gvkzhyxrf.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gykviiwqd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gqlkuuyns.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gidbxthqu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyvrjleqc.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gojpkhsbw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gzxvintbq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/ginnuemer.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gqrezyvdx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gwfnoramp.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdkcunnxs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gpddtmhbr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gcbuqaxfm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxjyokncb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvpwgvpfz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdylqlhmv.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gekibugoa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gfmxnwdet.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggpwoweti.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gzkhxtmpl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/geznynayq.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gfufminzz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gwqonvxjv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gdseuxhlg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/goonnzjjw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpwjtajla.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gwmbxseuo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gdvsucjan.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gcnbbxflf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gugvcbyxl.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gwoukincr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gehimruiz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/goxedozbh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gphyxczbj.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gcxfyfcil.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/ghrszlfjo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/ghhrmlhsj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gqmfwhgyz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gguxkxrgn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggcosorwy.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gekuvosem.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyxpgerpg.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gxxthvnym.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gftrtjhga.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gyrxzcxxk.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gdkuztooq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/glvglcqju.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gchrmekic.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gfnphafrc.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gmkjngdzp.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gkawiimzk.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gzadezyey.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/grwifvovh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gbombfxcw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gctynxdej.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxfrtohxs.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/guzlvhqao.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/geocvvjfd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gmazwrrep.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gicfbfgdd.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/guujcwvyb.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/grpzxiabb.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gugwrbzoi.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gdklchvra.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gzhopuskj.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gjfuxutgh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gmduqafwz.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gltjnrwkx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gntdxkfyo.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gavyjylok.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/golnkneqf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gujtsygad.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gaiigodmb.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gmawpjgvg.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/glhcvkbuy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gruvwhctd.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gintoxwkp.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gzupaseed.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gsnomxmeg.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/giqkclhpn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gohtfisjo.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gnyimbrwr.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gyubrvzsv.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gufwasgzv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/ghwauanux.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/ghtkwsexj.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/ghmkhbivx.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gnmzdlhdi.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gxubpdilw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvkuntuax.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gwtpglgfu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gwrproezc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ggluhbscw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gzzpkigoy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gzjqkqipg.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gvmjbrrql.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/glbggdblb.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gvllnqpoq.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/glfqipfti.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gdikyyrvd.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gudyrcyut.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gckisqezs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gunhrvqid.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/goxatqjeq.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gijvwqxgk.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/givtctutw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gndcffslb.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gikztcbzo.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gwrvnlzhx.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gaifmmllx.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gwgwujptt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/grgmvaswz.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gejmtzqwr.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/guxepcgak.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gjlexwxig.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gvrjfoeyy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gjotrokys.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gbrpcvbxo.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gqqgyzyyc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/ghnzldnxc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gudokbqmk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gqwssltlt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/grqsuqrrz.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/glubbmdgm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gzwxdvcnf.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/golldcvoy.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gdylkahmb.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gwbbvurfg.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gzjjtyhsy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gtwfdcryn.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gqnhqpegu.sHtML


<!-- 参考信息 -->