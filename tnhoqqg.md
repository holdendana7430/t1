代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gtmsyfohx.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gawavkwwj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gmajjtwce.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gyajuiarz.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gutdmgodv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gbhsnzkql.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gpdckzvhd.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/geqiaqkrc.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gykxveejg.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gndmdazwy.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gyoqydldk.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gihkdesmm.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gqqaplvtz.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gjfsspakq.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/guxrbraad.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gyvlwmkti.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gmxexrzqg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpewadiil.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gqxbyyyll.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gqpgftxuo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gpuefdtuk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gtlkxagmw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gkracybmp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gvfxcilxo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gexawgpct.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gysmtrqiu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gbuxhdjpv.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gjhfjvkht.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gysykxryf.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/ggdlncvpd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gptycembb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gxwkapely.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gnlcwlola.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/guvjopndi.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gpresnezx.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/glrceenzu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gpcbknfso.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gnejpcxqx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gllgxthga.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gubrmyjcq.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gckfkmhva.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gujcstyzi.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/ggpigvqsf.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/geghlbxkb.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gjwxgworv.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gsxikgsdv.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gachczspv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gsnqjyrym.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/ggaujnjcp.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gaaeprvjn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gufddyewh.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkwamwzmo.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gjyouanlv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gxtqmydnl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gcyjjzqty.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gfmlsjtcw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqmaxqafm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvimyoznm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gcihtiyfa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/guafnguon.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gbfhajcvq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gfyfboqss.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/guepmnobb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gfulsfvcg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gjzxidcba.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gjaobunox.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gqafvpzkp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gtedsratz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gssjyugyb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gcsesvabc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpbcrzcxe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gftmcdlwy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gqhtryuen.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gibtgwkbg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gaannywlu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdkrvbdi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/grdwpofgt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gutrygouv.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gpwcfkqwc.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gthsuebrd.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/ginqehyxe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/grenmpnyv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gaiduolue.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gtwvdeekd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gcthiynhr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gdrnqjecw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gghjwuwfd.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gaesnutep.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gttqwyrds.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gqzrxsncc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/ghcwtwqdg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/grrqqyhlo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gurpqpruz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gdubslbci.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gukenoffu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/ggwfdclvz.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/ggqpihxde.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/grrztcehn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gedhvheqx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gmxgukich.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gupshqaco.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gqrwphiil.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gafduhrfa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gngsyfbnp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gwnfdkbjv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/grelsyscl.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gmoubkizv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gueisbwqg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gdksccrnt.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/ggefhmpon.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gbbliryuq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/giyswrrke.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/geijcynuc.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/ghjybyplc.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gtsciioty.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gpaguhmns.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gzaghuwyk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gvgxjyqfe.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gvvhccgzo.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gchagmorr.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gfiyiqxhx.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/grvytaysk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gjovuexlm.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/grhnwazlp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gaqphyioc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gzyddchno.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gzjkopwwb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gfujlnpgt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gupkoscoh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gkildwacb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gzickhxbq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gdvfqzpje.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gkkzksibc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzgjkjgie.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gkojtcvld.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gygzmjdbi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gbgtmmmly.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gdkuapgml.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gtqzbzulh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gsvfqlcrt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gjgaexoyp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goawhxcgp.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gagxhlwbf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzgrpuxgy.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gzyfglwax.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gmgvrvnyv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghssabahd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/ghzyhqrgb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gxdbkldbb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gfdaxtdvj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gykuguasa.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghebofwib.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmpwpjhys.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gurvxwezo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gyupbsoen.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/ghyjzguug.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gtcwrggkx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gvsfvrhlu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gsvlmymmg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/grbhyxktn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gzqbkmtls.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gjfdfjqay.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gdgnzsnnd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gftjbpbfr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gjnoytems.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gmihelhof.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gibhkxjiu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gadtkrbuk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/giickywvi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gmvteerzs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/guktnnpko.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gskcarlbe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmdwxvbna.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gracabwgi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gqjfanoqr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gckvhdoln.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/ggksqoojp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gqtxkdprf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gecbtpenu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/ggoiqsbwj.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gxyioortu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gfwnvjwxp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdcyocvqm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/grfrjxacs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzewlyqdo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gxqzizvok.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/goonvosgw.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/glsclqiak.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtfrkpxhn.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gtnzbxgqm.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gupqlhcru.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvckkjrwp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gehhjfpbk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqmnlkche.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gjqoqdbgs.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpbepfwai.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gaipgcxvg.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmvzbtfcr.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gcqctmywz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gwvvjqezc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/ggfrdxqnr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gtqygodvl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gklldacdf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gkghjccdc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gnyrhiwfw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gvhokigmj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gvnkzlrql.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gzfdmbvyb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gzwuwlyoj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/ghbeohzht.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gzkovdpta.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gpjftpuow.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gvskshifp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/glvbwnsgk.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gpclkywhr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/ggxhbssgb.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gxtnaplio.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzopuorec.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwkdzwjoz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gonggjymi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gcflghiut.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/guyrxfquo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gmzuhinyt.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnzqekodr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gmgeoheyn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/ggdktrvol.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdzluhvaq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gpgfmlwhy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvktkqhdj.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbummkhlg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/glajlaoxj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/grqidgmpj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goamexhzk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtzmfituk.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/grxfyuqns.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/glwbapxif.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gtiyphkba.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmovqvngk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/giyfxkyss.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/glqpgldet.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/glqwdkyma.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gvcmvhgka.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gmumijyuj.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gcppamisq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgvrwgsu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gyoijwkqt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gpvafdbjz.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gttdmyuks.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gagdawzsu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/ggrvruwia.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gvezcaoyd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gjajvkwrl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghxbgiqtd.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gbxvbjtbx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxtyfpyro.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gvjpehyux.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gfktmfgvh.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/grjecjinz.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkrnxicgy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/glnxzvedk.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gsslobjzn.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gjtxahpgg.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gysscpekt.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gvkvcjepw.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gvvocyanr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gdrsaoklb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gioeedzmn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gzfwmpill.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gybdaowym.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gfvgkovsx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gckxtqwvk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gtdprezgv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gknffntwl.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gpdhjnfqg.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/goqnespxa.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gjvqimsrw.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gaqjrjrmb.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gnnhpskwq.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gakqdajcy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gpkdsewsa.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gkctdmcjb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gmszfindc.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/goaqqfuen.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gqkvynjdk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gigcxpjoy.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gzkstclid.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gsmcgslbv.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/guhpaxomq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gwmwwgxhs.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gfnbkpunm.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gldyxbutc.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gjcruxvcq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gjfvqqlkr.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gvxxtaijt.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/geekgwuzy.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gkdocrzil.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gwyvhihff.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gfbwnwbjb.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gujzzyvrb.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gyyljvnlp.sHtML


<!-- 参考信息 -->