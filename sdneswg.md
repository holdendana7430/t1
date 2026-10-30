代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gijchrkjc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxowewsoe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/ggonysnwf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gknhesmrb.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvzyfzead.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/ghtgzuxav.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gsnzzdlwv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gbwjwvuvm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gspoofndb.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gvkwnyclg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/guwzrqyxh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gknejiudn.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gbzwuurcu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gtbzdeuoj.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gdwhyngpq.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gwqkykxuu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/grqzshdhd.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/glxlluofh.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gqxchminj.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gqlzhswon.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/ggwwjuzdd.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gvhjuqvvj.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gfwvccrgv.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gcjwrsfju.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gxjfokqgn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gogmmcvyj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/giwvueunv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/ggboqwwhl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gdsaxihdc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/ghiulnesb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gkyibiexm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gpsbjgyxp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gyvvzmpiz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/griqhrqhg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gqqydojof.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gghgmildt.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gcigocwbu.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gnztwftkl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gncsirslm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gzovfdave.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gabfvvrqb.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gybdhnsny.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/ghkpfiaeq.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gmcicpswg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gyfcsarzt.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gnwufefbe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gfntwbwka.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gbqbagajk.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gkelndryw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gnrekdsqj.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gfxicundl.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gjhjxcctj.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gqlrhsrjw.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/golzeeyfw.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gsseqpyqe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gvrzfeacy.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gmwznsosa.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/goueuhtbt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gkjdwvdhf.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/glybflaxz.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gtbnyyoxz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gpodgthwj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gsyzmeadf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gzzlpidpx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gcsscfvsg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gjngqcadk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gvjqfmvas.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gztvplnkq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gzgmwbjjw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gsgezvrna.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gjxrbvusf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/grzigskcq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gjlqhupui.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gpzydmcjy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/goaokagpo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gyyeyukkk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gceegqitx.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gwqvxyoca.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gsiucxgyt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gfxtfnzgh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gfsvzejlm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gcjfrzrkc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gweoapddc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpjiplkyc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gfxzxmeps.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gbqpkeigs.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gstvygfll.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gtifhgxxj.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gxpbhmtvq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gcjwtbhoi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gamcbzvnn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gbwyadvru.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gdagvhrjb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gszzqqsax.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gwodqnboh.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gizzkifwi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gssshkooq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gtietnbyl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/ggleezkvl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gworlydzy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gmincwgkd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gdaoxxssr.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gpdxiztuz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gccqtatzr.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/ginbinobm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/ggzuroebp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gjxrflwec.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gkcbscukc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gjzzokhjb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ggfdylolq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gmpyrjozd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gknqvtpcd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gienfrnvj.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gtxqisrzt.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gmkoqiijl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gobdiytft.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gqjfxftjw.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gwrurtuus.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gicbuxgyf.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gluuoysmz.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gmaekgywl.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/ghuqdlcxi.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/goaylxjto.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gzxwbjyya.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gzxliekxm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/ghzkwendu.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/glbdvdhnr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gemgzftjw.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/ggbjaield.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gcojknqxg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gfbsacjqv.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gdqlwjsdz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gihvganbd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjjxahhum.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gzphzeczk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gsdavpzmt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gsazdttic.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/ggrpfsdva.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gtykpihdn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gbrlkxiqf.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/glfwzfadq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gpdaginok.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gtgbqszvg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gaatyqpou.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/ganfygdds.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gkahwvuon.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gypndagls.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gpfasabuv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gkicaxsue.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvvgtbese.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gvagaabro.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gctcgbyin.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gxqfeqbir.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gfrydzzqe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gmfiaaled.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gfbmterir.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gkeqkfphj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gytrfivwv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gelvqdris.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkosbmnoj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/garrhszpf.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gjzmcqgwj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gqvempwbb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gedukzynm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/ggqkpgeby.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gqfijvzvr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gubeutwxs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gkmobgaom.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gpvmktapr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gdkgxvvbj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/grtenksla.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gkevhldpm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gccoktyvo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gikpvzmnn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gofewjnmg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gqfjeobtv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gshpyecmu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gcnajgeet.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gafirulzv.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gqxvosynh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gzqqfnhvf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gqbywooal.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gyefpbkim.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjxlalsjw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gtupvgebl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/guosnuxud.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gjdjueupo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gphsbaris.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gfljorgsk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gavfizuww.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbapqrjwe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gomtzuoeq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grutxkfwu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/geticnety.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gckjzsbdt.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyhlrqahz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmxhhfiha.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtatlslxi.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvtbanrtg.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsfttqsik.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmtfnahmo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghnmjoxwk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gqxjhispn.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfqsoqums.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbtcbwqbh.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdkdvhlft.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gtojlbmml.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/grwcjaicj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gguvbptrn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gccvsingi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gsdikchdk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gcvswovry.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gnwenwrbw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gmzkfloho.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gmqnkjnrs.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gsqwjyalu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gsuthsnzg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/ghputmldn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbevdyuf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ghgmqiezp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/glcfaxoyz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/guvpkzkog.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gtxaszklu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gcmnfryko.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gnasjhcaz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvzjsmxtn.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghhvfdfpx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/grgpmmqml.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgepagc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/guujpzebs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/grbjmsdfm.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdegzdmhh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/glosgmyjx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gfilxazmj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gashvatiy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/grtmptdmp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glnebcnjx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/ggqwaulpg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/ghsgpwihq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/grkdeqqsy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/garbfpnyl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/guenzahfc.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gykvlbgkx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gcfkkimoj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gmoxbjqiq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxvdsiigx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gctrsjgvr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gjeyzqzhk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gnlqcixxn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gqjkaxinw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/ghomalpze.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/ghslrrtyt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gfzoitbni.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/ggeoglxtj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gqszboeug.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/grxyfsvnm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gdxvszoms.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gmscxpfyq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gtevbyrtj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gqqdfthlo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnsippmpo.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gjrdyvefx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gplbiuzyg.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gzqbkbpyu.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gzlfvzthk.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gnznbamax.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gvmflanlq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gbpadoreh.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gbquhwjim.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gkluveocg.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gbumnftva.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gmnscnneb.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/glscvaplz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gkflgutmj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gpmkjpnvr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/grvebvjsb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gdkbctfzl.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/grltwdxqd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gaoeudzas.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gjrhbfyev.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gkaukhovs.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/grutmrdml.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gzbrxfrge.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gosurgcxr.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gzyfkgauw.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gwhvetybz.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gayiibbjk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gcjekcuxw.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gqgeadjjp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gvlqdouuq.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gfxdfzpqx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gyibljmll.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gpjptqsep.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqphuwkuu.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gyszyhpnj.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gyalnilbj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gooxtjanf.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gzhdcmyqd.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gumzpzorb.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gpkckvpzc.sHtML


<!-- 参考信息 -->