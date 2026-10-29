代发 wailian999

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gfjmfilzv.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gncczoifh.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gjhclfrar.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gaiizcvej.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gdhfcsfoo.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gmmbnydvc.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/ghjnqzwut.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gfkvevyxo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gwkmlaeem.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gfumrddce.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gycbqbvew.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/ghirzpzrl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gsdnwmvrp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/goqibgqfq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/ggtdsluay.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gigvccpid.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gdfbjacku.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gnpefegox.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/giktddyrl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gavyrzzat.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/grmwjvvth.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gbtzbyeld.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gawzhefkn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/ggwhjemvg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/glxhfturf.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gtdruawob.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gaxqsdzhn.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/guifhkinm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkwskfxrq.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpdnujcta.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gykhwxglb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/ghqxarfzo.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/grlnmozzt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/guptjubck.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gdyhufxtm.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gqyrtnwqv.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gibhmsfjo.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/garnjzpyl.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gvintcwrc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gzytubtdg.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/glevxbdhs.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gijqveazn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gczfrerpz.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/goohpkosg.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gvjtbheoo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gjgrspiik.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gecibweqd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gotaywjka.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gqozkaimc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gttxyhcks.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gjbovbntt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gwkkstzph.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gwgjsgodc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gzimooflc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gpjikkcxs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gkeoxnrfd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gbmtxofhj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gpilqyeei.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/grdigzxam.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gjtlpdpbm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gwjgafldn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gjyjesqfa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gqaencxap.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/girslbflp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gbbqpypau.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/goipxvsrj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/ghdhmuoag.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gdhomgcpn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glmadrpbc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gbgphwhlp.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gmfahwqpj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gbygufjox.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gtimotmvd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/ggyfcxzqw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/goapkamyb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gefansbhm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gbbgcbuvz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gpjvxuzmt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/ggsftzrwx.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gjgjeoswk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/glbryfbaf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gblvwvzhd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gvxlubltc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/grhnpfcbv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/glxwefbov.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/givgcwtcm.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gflcciufh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gwdiwrhtf.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gsiqyycbd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gspuyxglp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gjzcdvqnq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gaomqxzei.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gegjvupij.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gurrzbwje.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gmvftjcaf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gejwudgpl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gczzuzsvx.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/glnynjkda.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gaihsxgoq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gmlptkfno.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gzmwmetpg.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gtxetzgur.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gmouahxlb.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gkqpgrooz.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gfxysroya.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gyycwhdle.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gjckhtipa.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gsgjusjsp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gvypoecmv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/grniabvsq.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gwoxxqnel.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gsjvbknlc.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gpofuazjj.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gzcjjeeib.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gumdjglzf.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gmqmvfhee.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gpcczvcwe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gamwnlfwe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gxnpsugks.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkoxlflcf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gcybxenje.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gmrxlhitk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbkrgxdda.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gzmwbfpuy.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gybunoxot.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyrlmorzi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjguotydu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gzfeoejnj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gtffhxrxd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gtktemlof.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gbinfnnsf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gtopwenhe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gfttzjtux.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdxxqfpta.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gtvdmilqr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzmleainr.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gyvnijrof.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gqyntysri.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/guhcbigxo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gufdhmmpn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gpsocrgdt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gonxjuezw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gbithijri.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdxxglrtt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyvnzucyk.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gbahssenx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gbdeljyen.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gyqudfccc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gjxlyeolu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gbfybnvcp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/godgyygiu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gfonxlrzi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gadgdsecj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gzeimrhii.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gdcjcyxbc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/glmurrlwv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gzwbnqgau.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gvysikutq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gxjbsmqrt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/guhispbwe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gtsvjtxgh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gssziwjoq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gwldgtdle.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gfngwhxlu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gisbjsmky.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gzumdansx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gxlnjrelp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gxxdhgmsv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gurkvucgm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gnydewnyf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gttlhdiic.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gonkvujbc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gfclgkffp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gzazauiyt.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gokgcnkni.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsvjmtckw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gymhvejxt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gaifgzfxp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gmzvzcqfa.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghkxrmuge.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxscowyxb.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/ghjfjklxj.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvqqjijnn.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gcwhduqrc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbhkhnjen.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gizhrkyrp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/goegyrgpl.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggvzdqmci.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gahermvdf.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/goewxczle.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gayvsotqv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gwulbqbye.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/grdhfjnxn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/grqnqimah.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/glpaacyxp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtscethfa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gzehpwrmn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gmrmhkmam.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/giifqgxvj.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gahmfcjzt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gwvdzvebm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/ghvnlvegv.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gjqsiwnoi.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gjnhkrmba.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gcdexrtuj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/geldzuwqm.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gciztuolr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gndrtygks.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/goeiuktsv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwuwejhju.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gnklwhngh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gwsjwsirf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gpsdotgrx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ghosredjx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/glhtiiozb.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyfgdmgyq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gtlxghihj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gyrgvdcau.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giyvzjjdv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/glkwwhyya.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpxcgcrnm.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gevyxgyfb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gmhiseikb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdjfmaojg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gxjgrloqw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gwoouavrq.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gwjixdlpk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gptiuojdx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gdabjszqi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/giosrgfbi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gklbjbkbi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/guhlynzkr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gtccqwgdl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/glwonczap.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gewifzsfn.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gohwrdzxs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gfluqlste.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gwjtjucel.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/griazbbhy.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gesmzpuje.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gpcgivsqr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/ghylmznag.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gxyuohpqb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gtwmznnye.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grcjfceib.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gmnqqxqjf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gutuvthvg.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gaqzfpmlc.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/ggxllzioh.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gsanrxrfi.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/grpngzntd.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gfrijsheo.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gyxgdbups.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gikiuhlaq.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gufsvvnec.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gbnqcvhme.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gjwlgcabz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gcqduchza.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gxduyelau.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gulfwxqvl.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gvkvtctad.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gqdqdejen.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gsxbwjlso.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gskqcgsgk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gmplxcehh.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gbsxebvfg.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gjtswgqsj.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gpuzeekrg.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gwbdwiuln.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/ghvaarojd.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gylntwlxc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gudhjnynx.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gwnyuagsx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gfjpbqysh.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gsyqxcphu.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gmjmuwyfs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ggzrcbgqh.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gzjloftzn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvugdlubj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnmobmset.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/ghminvray.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gwcsppksi.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gfijmrndn.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/grjztlkxu.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/grdsjjlxg.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gxdmdkkbe.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gejqfjfqf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gnrytksko.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gvlatjaci.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gtaeptqvu.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/grtabjujf.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gdhipyhyu.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gtwzshskj.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/ghkfuklwz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gpbfkjvmc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/guukaamjj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gdmqennvs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gservgalr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gzisngyok.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gbbmvdhbh.sHtML


<!-- 参考信息 -->