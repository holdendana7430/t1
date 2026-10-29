代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gxcbnuhzn.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gftzipoyk.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gjdkbizvk.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gjpaaqgzx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grgvlqrpq.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gezdzdkip.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gporylgtk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gwajmbgmu.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gibmtslqa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/geqfjrsie.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gzbxapqdr.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/guqngpslu.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gedpmgcvo.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/glljfdkvg.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gcxmmamdt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/glyxigbqj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gcztnyeqh.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gptzvplfo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gfvbmikcn.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gsbqmcxks.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gvnqzkoeh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gcvoandvk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gewftqmnh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gcthebxab.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ghlvorobu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gpmjgmzar.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gykdpxuzk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gtrqflqte.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gkmpfkomw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gflkavfnd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gxcfkzogt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gextxwbke.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgnndtdr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gjllvdgtl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/guphrdgvc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gnqykgzvj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gwylevvkm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gypsouwcz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gqxvwvvyw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gdpjhaeun.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gcnnhomao.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gymmvnnnx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gzwizbwrq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gssrvgozy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gkpzlxsmv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gupsbgrit.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gtwmbtckt.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gvlrhsesk.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gwffrmvdx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gqmzteohy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/ghtaixqth.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/golfqlogu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/glsumglim.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gudhpzddc.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gjruezbqx.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gksxlxudt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gsxxkzqbq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gfgwkzfly.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/grvxzbueh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gcwbnyyym.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gcpikcsai.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/ganxvtumr.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gcejwyxen.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gxcvcubjb.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/ghocjpufr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/ghfblnxwf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gvcootxur.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gxreqbbuq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gmnzgzfss.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gbnbgpeba.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gzujeqjgw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/ggmbtweoz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gtsvmxkvz.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gdkqmimkr.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gcvwicnvs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gplbocczp.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gncsnbowr.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/giqntennv.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/ggasfxiks.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gaqckqkqh.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gewlrxahg.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gmacdaulx.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gmfucfuqr.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gpywuehja.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gfzzxxupk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gekbamasf.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gkdzieryg.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gyfssfnrw.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gehcxwgyu.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gepdvclee.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gyqiulszc.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gfczogrzu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gqzlesbnf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gzbzazfjr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gcqfoycge.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gweosteod.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbactwhvb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gjsavteqa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gmzlvgxrk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzjgzibwi.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gcpvjqtyw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfhyhzfcn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gxzycfifh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gwkhtvjse.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gazjeecpk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gezozljdm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gtefitgcs.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gqbqdnwlz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gtycwmgke.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkqfraiof.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gzjlsetfd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giqefqzyf.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gekfxsvii.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gvbhmwwch.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/geiiuwqad.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gsqogqeby.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gkpjmttfy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/glggduzse.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gzsariptp.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnubluceo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ganxidkjq.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkjiapyvr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/grevbstxi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gbucbgaac.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gwiyzreoj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gtbvxdvlp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gnmxideuv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/grathuvjj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/glsfxavmy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gbefehbmu.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gcjnheili.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gegqwrzno.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gursyzqgf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/ggamcmijr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gpxzqobgo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gclpqekja.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gwffmijqc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gemezlcjb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gefyohyvr.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gxbsaykeu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gikozqdsv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gplqnxlve.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/grxnmxylm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqmjyassb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gubyzjwif.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/guskgxasy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/giwbbuuur.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/grspdmksi.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gwnemjqhj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gepgdmfob.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gftpqimtj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gepjlaomu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpwhvjmmc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gqvnlzvtp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gyxzdqdxb.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjhpfibgd.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpqqhripm.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gizlksegl.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmmbppbsu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ggvhhfdpa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjylyxzow.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkieomzed.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/grvtcdwtb.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtywlemco.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grxpopfum.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwdhthrja.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gnatbhxtv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gnggvxpxs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gjpizqevh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gcodmoknu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gbkvevhlt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/grdmzkcxx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gylwipcxo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/giorgcokn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/ggfdgzgry.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/ghuiyvthr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gqqnztoqe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gbbifkwlj.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gosjbbtdw.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gvyqlvvep.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gxeadrejy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gxjxjedan.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gdisrzzry.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gygtgwzvz.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gxtvjzxue.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsocnacwe.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/guymeigvk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/guaygmdzw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gybjnmmuy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/glrggmbyn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gccxnjusl.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gplegbnfw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/giregtnns.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/glqdzfvjt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gymdehkvc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gapgwksku.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gokeqkwid.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyqhcikhg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gkgfyskhp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gucviosus.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkyjjrmpg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gfsxnkgmj.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/ghzitcozu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gxbusuxyq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gauytfnrq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gfffeesjg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gerzmxmua.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gbodjjhup.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gtxfbecpc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gemumvxse.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gyuinfkdb.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gzdsivbrh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gdjlieebn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gopgwwanz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gufamknqv.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gglrdnmve.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gzxuawmup.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/ghhzwmjot.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gukmnptld.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gpqqpagkd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glfbvyujr.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gacypmuav.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqhvjrxri.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/getxeloxi.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gsltkqdhs.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gikvjhoid.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gbpxejuwc.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gctbrnmey.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gsolyafuc.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gdxugfbkj.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gfqgmmwvl.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjhoocefl.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/ggdqdkytf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gseyqomzk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gavxlelem.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gbipcnguc.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gswqgmvnl.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gpmakmdpz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/glwzformb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gvbxaowkl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gpobsmzif.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gdxjksfkr.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gmqepgdju.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gkncgxrjc.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gbvtnfcjo.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gneyvzvst.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/grdepkxmt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gtlkyhzbo.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gphyuesvz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gderlcfng.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gyioaqatj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gcjsfmgga.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gdlknbqbn.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ggndssyjm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gndpbxwts.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gsvbtndxl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gtdkhlism.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gavxghgtj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gbmwsrgrw.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gamgyhnfj.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gipqjmcyc.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvyntixdw.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gmwuwouxy.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gwpbrxjzy.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghifikbjl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gmamfkdwq.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gfvxjalfj.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvtrkjtts.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gphmfjziz.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/giupdgjwp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/guzrjbjjj.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gwocqgyca.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gbmntfeds.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gurhooyev.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gqewvepdl.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gjroloomm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/glwpfeadn.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gjnjqrkhp.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gswwxwrjr.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gidtgzwlv.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gftyxygui.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gpyekulzp.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gfvdahnim.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/glpfbsgeo.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gztwuentq.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gbmqequrb.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gxunlfazr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gxtiyvjuh.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/goviaysja.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/grspbgybe.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gieseybbr.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/grjunadcu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gswcwbdzy.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gaxyfzpcf.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/giqupprsp.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gdyrobbcs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gdsczfkmh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gtaraqigl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gsciydmyx.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gcaxwckxc.sHtML


<!-- 参考信息 -->