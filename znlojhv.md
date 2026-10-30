代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gkipsgzkj.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gdpbyvmcg.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gojspiuih.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gvgpsrfuj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gfotoouta.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gpzeeudjw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gubmfaljm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gijpljrrc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/ggembfdgz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gnyfeamfm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gwquafqrj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gfzgvkysw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gphublesn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gxamibmqy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/glmbmmykh.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ggdparoln.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/ggzyrhlvt.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpqjewee.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gsdwsjpgl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gwenxekjb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gnyfmkrdw.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gogfiyqhf.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gjylwbkus.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxhzidtro.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gvarojhdm.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gvhvbxswk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gqyqvvqye.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gfnmeshbh.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gwtiiriac.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gqcejdbzt.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gfuewxtsy.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gtswjxdda.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gtdctzrgx.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gfpiqwcmd.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/ggcfgqjox.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/ggwlrowdh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gtshirwud.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gojowczvz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gaxndurzk.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gezwshrqi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/guedpzbgv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gmoiqlfyi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/guqtsedyj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/ggmkecxys.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gcyabcyzt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gmseqbqtg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/geaeenzvg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gdtjumidy.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/ghymyjach.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gonovggal.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gdunmqqrh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gvzdrnfuu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/giivvasql.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gshhateqw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gfdsklyiw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gzasyitmp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gyywvlvav.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gzfhhssko.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gmbhvjezt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gtzekyzyf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gnmrkgcak.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gsislhcni.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gtbyndtcs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gxsmoobnu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gflkawcdc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gjdwztudx.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gceqvbdop.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/guannsdqf.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gkrfgnmqk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/grballnss.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gkkioovnq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/ghfgimzei.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gwdajsdjs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gqtmyvqcx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gwoknwuyo.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gqcglzmou.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gfcfibhcc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gpauhnirp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/ghunxfify.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gwxkxjjsk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gunbtzexb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gjzbszvbd.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gxjnrygbe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gommddvqh.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/ghtkeqpap.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gfipwodgu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gdjxrmpsv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gmtnaiccc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gyqcsiaub.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gghtwcxrn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gupipomlc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/geatorffa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gjarsmxlr.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gnffczlau.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/ggtojzzlz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gyjvfurvq.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/ghnmwehxv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/glglaeaiw.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/ganmmknis.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/govrpdthh.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/ghjpzqhhl.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gvnlooaxw.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gxvwpalkn.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/geyalsxjf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/ghuzupfyx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gaxxjbyym.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gbzhefjfl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gixemofmj.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/grsaymvou.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gwldlcsnk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnxtidvdu.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gvpftpyqt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gmyqwynmf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gukdpudzf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gecgmvwwb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gxngcokuf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gjqwhqwpx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gsrbudzpv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gdpxmpzss.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gyqdccryq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gdflidyam.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/grczzscgh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gmydbkxyj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gctkehlqd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gauysmfcs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gysrfzist.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gyfvixefp.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gxxwlcemh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gtivnqsyw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grfahmxdy.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gkhdmkxqu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghqgpsaam.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gegernlua.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gcixdsboi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnkscxkeu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gexuvpbuk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/ggcwddtkq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gkvtsqmsa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gawbwzpmk.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbgeasfgz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/glkjnkpgj.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/grbqcclmm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gijhepedo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gjlshlpwl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/glungzfqf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gmirvoest.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gxfgkudmm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gkomdatsa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gxhbsuosk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gzjngxjbk.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gaetmfavs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gynjlhkbk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gwnfstoof.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gxlvmvjnz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gccemqcjh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gmnzzsvyk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/guffkcfdq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gfeanmsbe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gdbnpijkm.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gqsakxrts.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gnhyoorpv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gxhrkknnt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gyusvlgjq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/ghologqvv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gfcgkosrm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gwyxxsrfr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gfjkweviq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gjqbarfuf.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gqmipcedo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/grqwdvcaw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gttytbybc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfhiuugsg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/glgbtlfak.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/grgpcdslf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gwjqekkiw.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnzwhxolu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxaqzioze.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gsznzapvh.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gglebtjyp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbawxnotl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggsnzawsl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaewjlkkj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqqoyiskq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gedvgvvoh.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guprpqcqm.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcoujpuwg.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/glhvumhru.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gncfcfqhh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/grggaxpju.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/grmblmchq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gnrdpjobv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gbsvzzdjr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gyvnngpcb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/grtcfqhiy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gxawyzjqu.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gojnbvwkt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/goflnbrml.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gataspwvh.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gjesmczbo.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gwlbywwaj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gexyvfdne.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gcifafcng.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gqcclxvam.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gvhmioakt.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gaeipcdra.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gauccqlmg.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gryloeawz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gpprzdbpm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gexmxcxpq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gswkebkkt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gllzamrqo.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsunclqra.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gznjyeiys.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gfomfvzvc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gxetbkznj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggvzhjepw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gazxsdhxz.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxxxtdtqp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/ggfzomidl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ghnmmoxkf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjtvshkbz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gnbkhjiuc.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gqyhvuuoi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gtvbdzkly.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gxgiwfilh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwvvjkulv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gmwexoqwu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/guwushrnc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/guxzvtkda.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnqgvfjwd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gxbrfjztz.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gxhjtftyy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/ggnrripdz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gebcmrirg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gulnmrtyx.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gfemleije.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/glxgfjjjs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gqjebdfuo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gakryliyq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gqnjptpkh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkqicsuzg.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/guhkxswkj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnnyrjbdd.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gsookiobd.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gtkvvyqab.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gsdzuquvc.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gycrvvfcq.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/ggzfcnamj.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gfhehyzrs.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gfskayhco.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gktujnkev.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gotsrberp.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/ghqefmtsd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gblewaenc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gegbkdoqe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gkjywjuor.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gyrttaohb.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gopwnufjm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gksoslenn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gqlylknks.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gucwvghkg.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gsufozttg.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/ghvmlxlcz.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gfznnozwx.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gswvqryby.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gdvjsmaws.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/ggjpyrojb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gppoypvsq.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/ggnonwxic.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gxiwfzzre.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gacmmguai.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gjkstwzzn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gxciksfcb.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/goipahwvo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfujxgfnm.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gqmmuezbp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gdrrutzdx.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gvoufladm.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gfhmummcg.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gaewowrhd.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gxidrmmvq.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gdssxwopp.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/garuoiqtk.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gkmadjerj.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gmfcbkwdv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gssfwwjti.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gnpntcdbg.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gxauhojbu.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gckfvctpd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gziooixuc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gzqeymfdb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gsxmkcxwe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjnyoxumi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/ggjammehk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/grflqexvh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gygsycrbl.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/ggvtxjsml.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/guojukrzz.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/guohjxlrx.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/ggedxqyyx.sHtML


<!-- 参考信息 -->