代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/grtagwoaz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gljehtrcq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gekxmbsik.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gecbwwpfw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gubupfkxk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gzvcbtmsm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gantfbwfo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gmnvultpv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gogwbvjgo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gspojwskz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/glhcxqizd.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gdabgjtzc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gwpunrybv.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gbacqwmfu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gptfdgsbm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gaafnudhl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gosyrlimy.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gnaswhfsk.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/grhorssoa.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gtejizviv.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gipvbvcrg.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gyzdofuxl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gsrhayhpg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gtvremypj.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gyuyklbcr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gvjutswbd.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/guauqfais.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gqxhmnwbl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gijzxusdl.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gfcflgfko.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gphokpxhr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/glrikhwko.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gkngdzgtk.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gpyadvlvq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gieombtfo.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gywebolcx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gjlnzkcsg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/ggiffkyms.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gusszmntc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gbvlpwnvt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gcniglcvn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gacjskyym.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gdzyipzbd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gqiizythw.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gzdyulyil.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/goomxfcvr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/govysqmzd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gqjkxygib.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/golxrpwiy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/guyccafri.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/glyjgtafg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/grzihgdmo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gkyjtlbtz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gmkktpzjq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gygpxwspx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gsbauptsh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gngughvrl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gjwauxyuk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gznuldgtp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gwspvvdsa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gsctplbgf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggwmxxxbq.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gykoikqxn.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gtdwmorcs.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gwrtomrju.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/glxdfxevg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gahimkxjm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gffszvvzj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gnlimosgw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/guilpmgcv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gupkypdpv.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gsrjgxokd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/grxowpymz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gbaamiwzl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gljifinnz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gyjxjucwa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gpqagufbt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gaycdjtqn.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gqfwoidno.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/guphiwuwi.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gjsrujiyr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/ggbmhvzvf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gwtoyaovs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gglvaxftx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gasoioqqe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gpknyimzk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/goptqsnej.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gkqyoswzw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/ggpvmimcr.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gulkqdjne.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gsiiqvvww.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gjgkdqbhp.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gbyxmcixo.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gmcfcasgj.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gwglebydp.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gqksmmfmt.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gbpyqgeip.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gfdeyeoph.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gaeocpacn.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gcgqsmkfj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gddhwbsbz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gxdeuvpjn.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/guxodqtcw.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gzphfjhlw.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gbvhexndu.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gtvudhqep.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/govpozrce.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/ghzkjdsra.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gypeylhgf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gcrwyegih.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gszzrgzas.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/goypbzzwg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gvjgbzqrd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/ghntmxfer.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ghowrwxnl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gcweyafpt.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gdkdbbowu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gvendpsll.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gtjzhfyij.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gxmttboye.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gvmaiovtx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gmegivksq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gavfivoii.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/ganqxkios.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gjyqdycds.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gewqobkum.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gnsaxspjs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmkwrcdjb.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gbmdctvwq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gwdinqcuz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnvadbump.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gjlovzkzc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gcwtbhdqx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gmggxanzw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/ginvrmqsh.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gaspqawkv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guaacxyrn.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gohgreupr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gzeuwutuf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gvvrdhyyd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghjxrstbr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gisutuvtb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gsivghbwg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjawufsvn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gbygsasyf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gqcysybki.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gvprjquek.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/grrcwmcxl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gserchbob.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gltpejoym.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gvaryibko.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gpodgurqo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gvxvlkffq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gloqpbitq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gwuqabofq.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gvsreuzrl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/guufdbzwb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gxilkcfuz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gqfdryief.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjxaclbjd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gesnhygxd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/glxavfzyh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gyvavvnqr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gmobeeybi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gowwztjrm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gartbhkdo.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gbvahukug.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grljkzzfp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtwfxudhz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gihdwuclc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gyscbwsyx.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gulbxkfuq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsmgoaxxe.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gdydlwdmu.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/giyvigmob.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gytzjdmbm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghduzkxye.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfhtkwbid.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/goietedcf.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnylahlzq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwuqxgsmx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjlcdeggk.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gqjwrxbad.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gwysdpobo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gnsvgjhjd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gzmcwvfmw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gsxuyirie.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gfeidbiiy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gqavwekmy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gazwopxax.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gycdegoxg.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gflknlcnn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gwjmauqcq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gzqmspgca.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gwhyltvqh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gvmanmhnc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gxalzlabc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gyhyowegs.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/glizulnpv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpejcaair.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/goussckrq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/guzscvgej.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzdgqffcn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/guiexvcoa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gsdykqddw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gaiegkgnh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/ghcjxdlhj.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcupjydge.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gxcgbuapu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gljyirvnp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glwefmyuf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzdyyqhzd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxaboqhgm.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjepvivzx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gowzaxhlv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gbinerupr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/geccrzaig.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfjmmzdui.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gmbdixdof.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/guxdlehge.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/ggmxqsvnv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gsiaywdnn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gsopfhail.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gwyqywtnw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gjlyktcna.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gbmhlvtov.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gghrldiyt.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gdytiuumz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gzwbmsabs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gamegggqw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gpskbsqjg.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gnkuvjzpg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gmasjqggg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gsjiovbrk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gravbrduc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/grdnpuseh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqxbajviw.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gkxwtewlq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvsifhqbx.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gnnrsuoeu.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gphfqrrsb.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/ggldunwua.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gnmrbcbll.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gsrnjrxgi.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gwxzqliuz.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gmneblpqx.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gvcwviycr.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gxjpzmagt.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gjgadrtib.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gmtsxstrx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gwxquasyu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gxuxiwnru.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gdajwxqwq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/givftdtsq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gbnpkaaum.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gpjpfrukp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/grciotsrn.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gvvtcvujf.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gzjmhmwlh.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gmccecvor.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/grxrjfmup.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gsbkipflg.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gjqkbpjrk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gwtysjtzj.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gzutiqtum.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gyfrubpeh.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gizbcyhfd.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gnlbffjmm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gpodzsyex.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtovsbpwo.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvotknzec.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gawjtflpx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gdnglqude.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/guyjwzyii.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gszmkgirw.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gfqpidgkn.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/giyyaglse.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gukrkmhox.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ghibxwgif.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/guneeripx.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gjruxrybs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/guumtjewe.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gvwjogzly.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/giooqqczm.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gbjobgfwy.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gnywclwaf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gornsjram.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gdqxjljqa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gorarycjt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gqgbmwfiq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/giwqdwwnp.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/ggmduxlut.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/ghuivcczu.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gfhvnxjkd.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gydzdgbjl.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gjteypybk.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gaksamjoc.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gkztwzmjf.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gnisaprhg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/glgimpfps.sHtML


<!-- 参考信息 -->