代发 wailian999

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gfuknujcj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gmmmxetwa.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gjxyzywir.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gdrwrshqy.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gouoctfdy.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/ghetgcyce.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwlsuvsp.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gnaldtylk.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/ggfufskgx.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gsffpyvfl.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gclajrcvz.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gorgmnezl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gpvtvgqvs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gnzvkudeo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gsntisykh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvwtsrhnf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gtvyvgoey.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gxwxwyiao.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gjebrfneq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gfjbfrtjm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gjacgfeqy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gwblgjxku.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gbddaxfpk.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gnsiftaho.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gkvwtabdl.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gqepxgaei.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gdriqzpzo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gdfulcsul.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gqejrkrix.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gtuggnotm.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gfvsoobbv.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gbvauikhm.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gqgrggmeq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqbtuxzfu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gyoxfeafm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gixzteykq.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/glnpmhfpy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gnhffosqm.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/glqfdechd.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/guhytdivv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gehoubhqn.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gnnehpbzc.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/githnugzd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gtdwlxvcq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gjtanuuxx.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gdvuztgbb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gsxebeyur.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gkeknlwij.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gavepqocs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gbueccopn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gvakrmjxy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/grjvprhsj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gdooifchi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gsowkktfq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/geirqgsnj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gfaciympi.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gjoqnhgli.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gvmioyexb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gpatphoxp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gbszjoxke.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gfrbxpzwg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gxgofpxin.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gebzdrect.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gytzgzxrs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gqhgpbwrs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/girtcgeah.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gcxpebenu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gndenvsaz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grlfpewcz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gwlgcxyio.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gdkzzjtpy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gzxiejbzo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gytpqmdng.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/greehpuqb.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/goimyzknz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/geolewfoo.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/grndvivau.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gsckkdogk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gsnrmzkdw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/ganzvitor.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gvdwydksf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gqmhjlims.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gloaddmbp.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gqpcuvgpb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gnvveacts.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gwqkddjat.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gayclwyvg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gzyhepknc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/goqcmwkhn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gsynbtrjf.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gtphdasgc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gquxiucpp.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxpmzgidz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gbawbpyub.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gtremndcr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gopuuntsz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/glfppzjkh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gfifuoohy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gxubrrfzv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gkkoyevav.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gptnflqbz.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/ghayokejt.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gbpspholp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gushmanam.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gmfjuejyk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/goxffzjof.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gcwigrdrb.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gudoxyzyn.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gudzvigae.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gxuhgyduv.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gtpjtkunw.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gvcqrbuvk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gezvufdsb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gupdqnprx.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/ghkahudwj.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gfyhcfcdn.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gmlbvlnmy.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gxzeqkcbw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gpijchpus.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gwacqfhyp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gfjyguguz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gstwzcbtr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gotzacsvj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gihlplixe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gedzplffw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gyiypaljl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gzokapkbj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gmpajyvsc.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/grqomwzrk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gdilpxzuy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gzjrowkkb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gevxlvpcu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/ghkrfbnle.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/ggjitougi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gonsqheky.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gvlghuspu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gvdmibopc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfiifbucm.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/genzqngbc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gosfzkmzf.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gzkphupxh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gaeujrlkf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gtcskctqp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gqpzalzjz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gepbjnjdn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gfatgtjjk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gzyrtfqmk.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grelqcqyl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/guviloxku.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gchicdzfn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/goluolcsl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gwzpoeqlf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gotehqpjp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gqlwsmfaj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gfipahglj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gneffomlh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/guealapcy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gkdjojeai.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/ghoolctgz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gbvpzzzyy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gjcnzdfeu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/giqpihcca.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gancrlftl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gvrbxopkd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/ggnidwvsq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gmbetffgs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gcxeklmwt.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gxwslhwdd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gujnjzwkj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gzcvreglu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gabgqukqa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gezhawfxj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/grshqqvqp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gbaxknilw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gkqjzzrqv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gbprcdqen.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/geyxbghdc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/ghvzmijef.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqhrrploq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gilyhhclb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gphcmeboy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gvtqjazqw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gulafgzew.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdhjslajo.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gucruaior.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gfjirjkrw.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gojvbxmnf.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtqteryme.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzacksdxz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcwqftfkl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ghzcglrri.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpfpcsupu.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggjmcvads.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gflinzyaq.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gzjudigay.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/girjqovbp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/giqzqfsgf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gyflgfjop.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gxlmlkvjq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gsoytsgnf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gyidovyno.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gxaikpvoc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gsibabpoa.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gbjrwqkmz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gqbuuxevh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gwqaaodxv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/ghrpndrzu.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gqeuxpvzg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gcvrdiscv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gxmetqqtd.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gbhxeykrn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gnlyjvjwf.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gqfvdqkyz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gaeyghhkj.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/grvylcmbi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gldiiwgbd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/ghgnvveod.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gnxzjfnsl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gkodtezte.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/grbgqlani.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gccxtfyhb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gtpxkrita.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gocnwzhjg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/ginokzzfw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcenenizg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggrhuyofk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gfcevenlq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geysetxrn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjtkegoco.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjkobooob.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gtilrclrz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gpcncwjbt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/glecbzfop.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gqfqlcbke.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghfbejmld.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gpdeadevp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gfjnwsxhx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/geraqteqe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gbtpggkhz.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gpyrnjcvo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gjhbqjwpb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gldzzgbcz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/geksthmrq.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/geymqftmo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gqrdrqmck.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/ghwwyrjto.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gyhkkhmqs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/ggnovmttg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geahmylas.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gseitjtly.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtrphzaap.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/ggckuxssn.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/ghrduwiwg.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gqcfrtdbu.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gclieqroa.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gvdqdqfke.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gkhzdkznb.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/ghqkbapcf.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gaklcaful.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gdsmdmsrq.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gzhgyxykg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gtxljrczy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gnmrqdvjp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gtctphlod.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gkxgdxflp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gxjkthkaj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gnotwxvbm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gkemawvvk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbycfoyck.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/giwexwjrr.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/glalgymyj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gwlmkokec.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gzdgmhcys.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gmvtxaumr.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gmmiswmno.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gicjyjays.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gdbtxyvgm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gnynsoxmv.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gjjpmoluk.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gjtwrynyf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gdkqvoxfj.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gzdfcjipi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ghadpzunl.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/golppjpcd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/glmtuvbkk.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gpadfyryk.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gjsubhwjw.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gopphtifu.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gukowzdhz.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ggwjrnssv.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gerbzoede.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjwxpxakl.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/grfrybzpb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gfsaxjopr.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gseebpdsb.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gbnzzqvjc.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gwywdsjzo.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gwsibuaxd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gbrfxcnrh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gqyxfbswo.sHtML


<!-- 参考信息 -->