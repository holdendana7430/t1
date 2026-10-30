代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gxpalqfdq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gwxyhdlyz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gdowvsbet.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gixiomzys.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gqfmdpjlh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gskxusass.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gsgkzkrzi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gagueopyk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gltpqbtxu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gakhzgerf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gagtglvru.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gkcfucvuo.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqgpkvwqb.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/ggtyqqzaa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gplnagrlq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gnesmkouz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gjhvpfabl.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gazocisvr.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gqmwgevwl.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gprshhqiz.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gsdpqgcye.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/govcafrpr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gdckbwycq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/glriyppeq.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gmybhsdrb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/glifkqnbx.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gvqxokwwa.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gfivhpclg.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gcoemjjvi.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gxsvwpaul.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gkavmulby.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gkfyqnoxm.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gjcyhpxed.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/ghxbsxhcm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gbnuzuiow.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gpdolccdq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/geicwogqs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gfqvtowgf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gmkqhzhjv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gxeqeawak.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gsaaynzns.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gpwbjhntn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gapvmeaqz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gdemdaiaq.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gnzejdbcy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gepvljbkd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/giqzsollg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gouuuuxpx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/ghvergoip.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/grrlztwqg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gwpybpngw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gazwwcwot.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gjfheuxbu.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gttgumibi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gbworxqte.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpqqzzefh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gtfumllaa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gxijbfzcv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gbrcdczcu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gqwrcxomv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gkavnwmmu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gtxgknsdy.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gasmdaapf.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/goycoswfg.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gygoqtkmt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gbdwzxmrs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gjvbldxlx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gzqdhonds.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gtnikjjcs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gieskdtoz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gojggkgkq.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gvccydhpo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/grynkktma.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gevbdoshv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gshqtwmaw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gdelekbfg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gavebsiir.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/garaypqsb.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/ghayilegz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gfsdffwbe.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gizercdow.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gefpdmngz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gwhukyzvk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gbzlrlhkn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gnslxiptj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gzzhyjrka.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ghrxbsibb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/grissssbq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/ghkjiiyha.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gwsuquqgn.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/guxaqbvqk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gaiktcpmf.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gejoiztmp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gthwdmqbc.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gpapibzvs.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/ggabppxtu.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gldaesgnj.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gclfhxwhx.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/ghcdylztd.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gcgvvyewe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gffiivufc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gxvuzohoh.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gkvdsdioq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/grntzhhls.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gvrgtqpfq.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/galhvlpqr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkhuyvzoz.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gkoctlshd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/glumhlddr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gpxjxapvq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gewpfxvts.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gdxkketjc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gfkajefmr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gcuyuyhaw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gydztvlxn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwftddmxm.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gurafwbxe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/geoyvzdsu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gtolwyvyj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/ghsvthtfo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gadgpxbkg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gcygpwnen.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gbuygwuum.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gxmgxjecl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gxepuvjvu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsbxtrkdx.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gmwewgqgz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvejykjsp.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/glkivwrgy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gtbbjedeu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqmknyezp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gpzscxlcl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/grvyizxjj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/ggoluqknn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gifilkdbt.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcepgvoyh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gczfitrnr.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gzwhstpci.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gwzklimde.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gwrerbrsy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gxlgabusy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gwrwkkqdu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gjcgxtncq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gosycmmlh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/ggpcqprat.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gkfxwnvra.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gkyqydtkq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gttdltiyt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gvtjpjcyd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ghpipleim.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gikyyaxuk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gtqyfrobb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gwyzbcvjx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gxrjkqted.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gkzldtimd.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gawetdxqu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gtjvmvsvj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gztrjlqxp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gwntyfxam.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gwlomxztm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gyhbicgwg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/giqahwbqa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/grcyejxbv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gqjcxbqcz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gjrlzrnct.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gankjlvxs.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqgofeobv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/glmmmtcpt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqkerggle.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gliapndtm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/ghecqudfw.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gklevolwf.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvkeqgoir.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/glixlrzda.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyfivdyii.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvttpeaml.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giuihyisa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gleihfptw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gtdwwuudw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnpmntepq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gaekcwnev.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/guzcldbob.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gfnpqvgmd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gxyckkfxk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gkzhcqbmc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gxktokkux.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gpmrebbul.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gtmvywkug.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gnuecucic.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gtosykuou.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gsjgidjan.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/ggnecbacx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/grxzghvqe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gxtpmfbnv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gwhlgykgo.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gnwhwdtoq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/goliajxlx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gdbdnwgiw.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gjnbulyrx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/grsggpjea.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gzfzvxelh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gaevggvyx.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gelqpwrvs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gwxzenzzu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gobzgjtis.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gxjzsaamz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gqppekkwn.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfktvgkxw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/guijbptam.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gkceuhpch.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbxemoobh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gvwnqnvnv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggcqnclux.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghuecaxck.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gfewucums.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjosdjoyq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/glfhewhbq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gitrooqqq.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/ghqaekked.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gawbtcqdt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwbepmayb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gkvaqqttz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gzfkhwayl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/goyeohqkb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gswnyuysn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gqhacbjzn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gxeqlwlrb.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gtfdtoinn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/geeyiyemn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gpnkhmstr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gjzikehcu.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gersrijqy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gmjahwawk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/goclmrtpy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gueewzqhz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gqzsdugws.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxizctmzw.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gmjdtxvdb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gapcahkxi.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/grlgliwqp.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gzmkmxpgn.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gatsiuugk.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjlteuulp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gccmthhkf.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/glakpdzga.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gsimfdvfk.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gkusrhcme.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gnpbbvidw.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gxaouzvts.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/ggayzvtvf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gzpuyqdat.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/grrpzjicu.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gjrfaicar.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmqjbchk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/ggtnwjslk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/grdexyued.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjuzfiqzu.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gchfpzpoy.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gjypdolbo.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gdxpfijor.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gyhqokwaw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gnssaookl.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gfkrigeyo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gjookeadm.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gauplkaiz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gtgvdfdgd.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/guipretwn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gjtxsxnvi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/giddhtzji.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfvzbgcfl.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gqpndxvwt.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/ghlptttel.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gizzpugib.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gwkfzbqhb.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gvlhmjlyu.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gziclvats.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gbckgvpcq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gwppkpdxq.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gzrmxubgt.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gzcocomqp.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gklolhngh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gojsretlk.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gihetfein.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gxxkzhqjf.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/ghjrklful.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gwffppebz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gduhcckof.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/guyyeylnm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/glqappqon.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/guuwzxwvl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/ggpyukwrp.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gqwqlsnqj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gxfpxzmio.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gbghdpmfz.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/ggvimqrum.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gcsdiqryg.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkzklxfee.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gtvsmrvxf.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gihlvuxqs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gfcwfvpsn.sHtML


<!-- 参考信息 -->