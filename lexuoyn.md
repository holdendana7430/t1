代发 wailian999

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/grgppiqeg.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/ghyiovbuq.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gtsexundd.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gluymznws.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gwdpizryl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gcqiprjgf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/glrrdrekv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gnolypggx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gjdotdrtg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gozimxslg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gsrauiken.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/glidgexol.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gvpppvdyk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gnyjfxgfr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gqvrxokij.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gctztjkpy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gksemfqnx.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gnoirobux.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gqtiiblxz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gexgqqnss.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gzfoditun.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gbytjnmor.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/glbhojpim.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gfttdcbaf.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/geugvjawc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbnvbzzkq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/ghslbfcpf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gofvrcibb.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gnwbgvwgi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gsctungvf.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gjjkqierb.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/ggfawrhvy.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gwsxhxfnc.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gbuzezwbu.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gcqhkprmf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gbtyzqdyq.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gpzpzakxh.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gahqmuuga.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gdyspjqig.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/grqajhwiu.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gigeukfww.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/ggracgpfn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gtgtmowjm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gpsoerykr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/getcedjft.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gyhvikeoj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gcswnqmpl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gnxkmvvnd.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gaficahky.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gvvlxbosv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/ggqptdufp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gntbuvmbn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/ghewuqglr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/geagyeamz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gtuwbazmq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gvratxolv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gghziduar.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gwwsglhbj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gglwttrgh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gmbqercbk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/ghhiyslcy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ghadocatx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gfcuvsrrq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gpqjagxrz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gtdimwnvq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gijlqnjic.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gjoocwibo.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gatfyaspd.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gthcchpjz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gridekwpc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gruojqrqw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gndovsfhr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gpmopmbzw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gmqwfnmqu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gxbxjzjhl.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gkhvthinl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gmixwbotl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gqethjqat.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gcrnisovn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gzvnmakzz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gbuappbzy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gvyfiepzb.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/guweermiv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gxmtgnhmr.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gtlhamqaa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gpehqmrif.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gjzgtaetq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gphhjeevi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gkrzpehsc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gmymugtdw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gihwotiux.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/geziutpgk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gfdhjxgca.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gwdjkpjkn.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/ggkucdtay.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/glbnbkgdb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgbtlecl.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gokflrcsd.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gnwurvxgv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gscrgfqoh.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gfpznntsj.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gwfziyrqo.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gnnrzgcxh.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/glxpmcppl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/glkmfcqvl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpticvezl.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gkgqwxxxm.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gcsgtawnv.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gbeiemtkc.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/grdfmafkc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gefanlbmb.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gnkflqdbk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/glbddfkaz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/goxtjofaf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gpxjzybfj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/grgugtkjd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gvsevlgjd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gsueogzsl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/guxhwrmtv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/ggybrnmvp.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gabmoxdmc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gtthrcbwl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gjtwcgfty.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gpeeofzxm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gngyrkehw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gwvqrtbjz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gbgmxbeqj.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gaovicxpy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gphexgkxy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvxduzzjj.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gyblamthi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gecihjvot.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfsvshcve.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gxlnzqgio.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvstzqjcl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gizxlhxsh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gtmjgqcpi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/geldjnujk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gwkzkxdjm.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmcoqmcuf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggrlxxsbz.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gflmxdcro.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/grhurshea.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gqqmnvdkq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gtfllkulx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/goepqzpus.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gvmmyaujz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/grliqypil.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gjkjooyjk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gvzcteiuj.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gkbuedkrd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gfzlojkyb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gzhcjjoym.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gbtoxixer.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gmajaswwm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gvvkkawdv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gzdtlgpds.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gsqnpbndk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/ggedgpzgo.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gzabflkve.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gldixkhei.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gwrfavwau.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gyhsjwskv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gubwpemhy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/guyfrwqmk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/geurjiufv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gslhdncki.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/giqwbazrx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/glogxosex.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gtqqnaiwd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsuobvgcw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gevvyckmv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtacvbfbv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gphyqghql.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gqxmkdmjv.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guljhidxn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gentbpmgt.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gllfomven.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkbiorbxa.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gitsruppb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzubalgtp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnoedyoxd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkuawkqtj.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/guymkaxgh.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggbryqtxw.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gqapdarik.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gjoqzebsp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gfpysmatr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gorvlxpjm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gdhdlbnuk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gplpoodin.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gmlsxielq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gtkhyrlmp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gqbeoavmf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gehadmaqv.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/goqavsozh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gogwlegaq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gedkajzsm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gttrsvsic.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gitdemedo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/guxeqsdje.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gayewmtap.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmdambtcc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gejkmmhlh.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/guijoafkn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvabbrnfn.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gwymeafqi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gibkjgldf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gxffetkan.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gtkjuhkpv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gjqhholxl.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gktcqaede.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gyvkzotvs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gzvyupqjf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghcdgkoce.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gymyfxihp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gmuuifemi.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/goddehszs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gxasuimvs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkoepzyku.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gfpducdom.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjzectlvf.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/glwuldyup.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gltnjjtrk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gepdbadcr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdytamceq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghimsqqva.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/geryzrnto.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gyaurptjg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvcukxxsk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gumsxmfqm.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gumxmbjxo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/glqodoqcm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gekkfusbd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/getcsvkls.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gtnmvguaa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gbnxhqoae.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/grbjzsmpy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gbmmkuxsg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gryhrcvoz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glivofpnv.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gzyklooba.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggkjrvbot.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gpgdrybfc.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gjtplgfti.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gyqawvacb.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/guxwpcrlg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwetdbuae.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gtwkxamvh.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/glmdqaomt.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gkqdiajed.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gemgbfrum.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gjmiqpoyo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gzdpszzhc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gkmipbxzk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gguutcvgc.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gabnqympq.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gissdlwzm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gxjaioncb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/grhcwblcn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gnlycupmy.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gypittnrj.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gnpltjaiv.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/goparftzp.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/glrmkrhfm.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gpprbnktx.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gkjjidvzk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/geuvdimod.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gwluxxizd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gdqmshkxl.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gkaujledu.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gzfelelis.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gocvqyjna.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/getmzkshv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gmrrozamu.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gqbdotboy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/ghppwzecn.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gvmyepxrw.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gmqeeodrb.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gpgcftdso.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gevdqmkzw.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gmndkeoag.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gigjlzvnu.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gefodhjzb.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ghlxdwacr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gpxhsljdu.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gscqjmxfr.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gjoewxazq.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/goknuckpt.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/ggdeymmcv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gziwwvonb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbwmafvkw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjpoegcqq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gmmfjktvh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gnbdtjxnu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gmofthrbc.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/ghlxawoxb.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gjlougrmu.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gwwfoobmj.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gzrzhleso.sHtML


<!-- 参考信息 -->