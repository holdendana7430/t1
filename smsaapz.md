代发 wailian999

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gnebxkrry.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/ghsqehxin.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/geirmwqde.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gqvnhopyu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gpcoljwtf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/glordptff.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gvpfkkjki.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/giwbjogxt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gbsjhqyci.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/geaepdkbe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gksjkzris.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gyzkafzjk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gfrnounto.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gmtirtfud.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gwygxrpzu.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gkegtitwn.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/govbgpetj.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gorqonyml.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvkjcqoq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gvrzzckat.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gameoihja.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gswnwdyot.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gwyfpxxkk.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gkcashmuu.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gsnnzzakx.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gobvidarh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gswueflpt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gcuzefviz.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gsjlmnxmn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gguwivrov.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gshvosury.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gjfpmhunr.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gmbjyouhl.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/glianrczq.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gaoctpwev.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/ggsxoaxpj.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gdklnglwh.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gmtdgscpq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gltiberce.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gjfkjreaa.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gnfcfwuys.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gfytbcher.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gcthuzsbg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gdnxixgml.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gtlgkyewe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gpwavdwut.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gstkgthkv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gvlobnmjb.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gwnfkfjfw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gehjunwwn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gvarkaptw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gtlhzgrmq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gqgaujaiy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gvqjmaklx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/ghscwqort.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/giddlmrph.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gpesmqour.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gqjcnmnce.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gmacspmne.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gqafphsna.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gvvewklps.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gcyqyqpzf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gbrcyrvrh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gwznlxcwm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gihwcakyw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/glhzspisf.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/ggywmykoj.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gkatnglmy.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gglntistk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gpsyuufya.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gbdqklnce.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfrdmofp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gtxjjnkgi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gzpprdnmt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gtsuncuiv.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gvqffnqno.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gnhechtqo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/guzhbnvxz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gtxhqkvkj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gntwgxcka.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gzjioxjnx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/goeurkxuz.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gohjnpbmb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gyirhvrel.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/getwcthqi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/grtdxlsny.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/guwavsgew.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gbusgvnua.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gmdclexkc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/ghcpwgmxw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gawniuual.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gybfwvvse.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/glxmxnazd.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gfvspkusk.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gvmozqdbx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gfyenughy.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gkbuxyynr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/geixbrigx.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gbfbefjvq.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gtzhcrejh.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/ggpdexvof.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gchszbtcr.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gfcbxzbjm.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/ghrweawsz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/ghuiajxfn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gwsuilolq.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/ggqtksbfs.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gktraekfi.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gapsxttab.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gqlhymzip.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/geefukjml.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/ggyfczgtz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gjkmpglth.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/giqwpewci.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gywuxdoid.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gduyrtqag.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gpcoioyvd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/glcrazbml.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gxxttqrbt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/guyfxeujy.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gcexmxivw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gktkptivo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gjxsdftti.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gkecwaawg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gycdagmlj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gqtxyxchp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/goceshwlb.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gajpkofzr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gtwklvdal.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpatolwvj.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/geqapzbij.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gttxkfknf.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gtmfhnugm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gjjodwfdf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjsyejfkj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gyjaqkcxv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gmpmggupw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gqutbunqw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gvivgczpj.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnttahfde.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gybynceuk.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gerjbfzvt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/ggidlkpao.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/glqfzoinz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gqqgoheqy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gxurztcgw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gixdjwryo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gnneslkru.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gksoirfxa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gvltangck.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gyhgbjuyf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gmixxzfio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gfgucfkbs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/grmruxlxi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gxgfrczrp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gdxmtyaqe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gfmrktbtf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gxshzqala.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gllckwcgp.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gjjqziynb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gjatnlbtv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/ghfiniirn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gjsntuepr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gauieiejw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gdqjuiyuv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gokzredwd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gibablmzy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gfnixycrt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/ggdixuefo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/ghpodfhjg.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfsxrbfey.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjyhrnjlr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/geffuklxm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gkrnsujhz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gkgakogie.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjfmrrfol.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gthrgusts.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gpohonxvj.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gigtegvbo.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggskchjqv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gippehjbt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glloupawt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gthqcwhio.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdnzqsdrg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdgidebfl.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghmohpaaq.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gdpoookvd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/grfenltuw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gagnokgkq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gschgyzli.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gfpvilkln.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gdycqvkzr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/guzagouoa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gbfathxij.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gkvmxsmjt.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gamlhygdi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gnxtexwid.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gtwbkbydk.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gjzaejjor.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/grghkhxkv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gnkqalfvb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjsojmxuk.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/ghjuivnyo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gygercabu.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gasblyvls.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzwhcskku.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gerzgryby.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gipcqweln.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gqjbscvbq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gtnoiokpf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gyyfkymdt.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/giaonwdjw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gqusnwirt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gtacqkxlp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcvwbdzgd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gojplnuyi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/grhwbnnia.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/grsqphfzk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gvzjyhzjl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvurfunjt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpbxmrsxd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqxwcsokj.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/ghaltoyob.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtcioafqj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gztrnowth.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/grwcbagzc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/grqsdggfh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gvozflcwl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gfwdkuhed.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gfefjjwqn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gdeadnkzk.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/grskfcqvf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/glkrubtpu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gwoxirciy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/ggxvompbk.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/genwwlakb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gbzobfwtv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gssvhgekd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gvfwhfuxv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gieygtdcv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqdyysztx.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gnqqtakhy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzpnnbkmw.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gmynwnvra.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gcmdjwkgg.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gadfpdfoo.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/ghdpwzevl.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/govdbjgjh.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gxndvhyrm.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gzcmqmahk.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/glivbqqeb.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gecdqyujt.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/ghgafgclg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gwxyxhivp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gtjbuuotm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gsdemnzgn.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gsdvfmoqa.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/grjzopoip.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gwwsunqxl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gqyujpvbh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gpjldlvsf.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gsvmpthaq.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gkofwytli.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gvrczgzst.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gtperwrdl.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gulkbzgfp.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/galldrzau.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/giahwjsbt.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gtpqyplfw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gemqxffhb.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gmijavhpv.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gwymiquxf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyyhhsypn.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/getwehnno.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gawjcgqci.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gjmwhzxzc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gszruunxz.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gvqchzmsz.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gpvazkmbn.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gcfakxooo.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/glcsxkllm.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfcehspcx.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ggqotcrcb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gckzaraos.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdixwfamf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gzetrvorl.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gajhdzqjf.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gcsfbgkey.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gtmfpxhhg.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gibmjxlol.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gdfawvmxf.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gjfayrjrl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gccrthqyq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/ginercqyo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gyymaxdex.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gayosffjz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gachbkidr.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gierksxtx.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gesjtalny.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gymohlnyx.sHtML


<!-- 参考信息 -->