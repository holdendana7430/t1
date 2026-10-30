代发 wailian999

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/giogbeklf.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/ggbjbihey.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/glmdovgww.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gmdhrwcal.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gvddceeeu.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gjcgouxqg.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gtkiulyhb.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gsihuugfq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/grlxxvlmv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/glopzdzjl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gtetoqffz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gvmlbojal.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gsgglxzxm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gfexddvqb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gculfaean.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gedvdttpp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gvflucalb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gwnqjcezi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/ghyarwhit.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gewycdufn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ghuhmfdam.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/glpsjsxsk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gyhsdsvjs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gqrhohojl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gdqixzacy.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gzmootlek.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gdijvtjpf.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gyjlduxat.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gmsdtmabh.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gmyrpwghl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/grjejainh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gavxuhzxu.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghlfzeaqx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gjirgkrqz.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gymyviekv.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gvrrkjgve.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/glqvsxpdd.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/grjapztvt.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gcufchxpx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/genrikoia.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gufnpueae.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gemarokob.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/geqeebuuf.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gmabgdzob.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gzixrteuk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gtiitjnht.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gmzeaybsl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gmpjvdlsz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/golqmvynv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gznfdwlsn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/guxacvrxn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqggddyk.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gfwewwkgd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/giuageewt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/grqjbwmwe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gfkcwszhz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gcutandrl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gxnqorqyj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gvnjitqgj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/geaxtxfab.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gmycgedqn.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gbgjubetf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/ggankfset.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/geetxqmsi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gnocpekzo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gqpemkram.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/ggfwzxzzd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gixyunucn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gvwkjmrry.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gwgpgjtmn.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gwleitxil.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gfwlrnemg.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gwgxhizvv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gbiwaqlkd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gctmzahsj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gtnmvsaos.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gmduwuvgk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gpiofplbr.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/grepuxlsa.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gbqrmmhks.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gqmbrrdsa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gqyibpaoj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gnimgkisb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gcojykeag.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gvdfyxmpq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gycjqhzrj.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gjmagogpf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gxuksozid.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gjyykmtob.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gnywprvxy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gjfupiqsm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gyclvtraf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gzglnvzff.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/goepgmzou.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gmlqsuwsl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gttcdxcxl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/girliehtu.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/giohfikph.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/getzoarwi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/guqpfaqxe.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gfjadntjr.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gpqubhcmc.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gtwojoiwx.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gulptgjsa.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gnypjcvjc.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/ghwehggkq.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gbrwketkv.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gemurrtzg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gkghwgjpt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/grtheftau.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gguteowtt.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gukgsnidj.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gpqfrrdse.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gqnxcpzwr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/ggknfsbgo.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gycrcvyes.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gzepwyfjg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/givdhgeve.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gexyyuyen.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gomczrxqb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gacroujht.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/geaznmrmy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gxcmqzout.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gkdhccwxl.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gghqueqgj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gvvhidtgv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gwgqcwznd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/glqswhmus.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gnefxgwva.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gpgszoaey.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gjdkeyfjz.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gnqwlaqld.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gidzztrct.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsavmevda.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gpzcofocl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gusluegjz.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/ghxcccvgv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gcjwhxmiv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/grpltsjgc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gesigywav.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gvpicaolx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gbggsntue.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gyciljskc.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjpicpbqg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/guudhntcf.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gunwbxqyq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gcvzhubcz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/goohkodwr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gdfrsbhxo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/grwirarik.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gbifmolwl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gsxilvgce.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/ghzigbryl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gqcnjkfri.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gzhdcxjmu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gltordcwf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gnlbfrvhe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gukaoylub.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gecnxtpum.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/guyeiruwx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gehcmhgle.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/ggdhfgkfc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gmfqtjjwa.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gsvihjayb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/ggnjxovlr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gjxxivwyt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gzpckhpng.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gpybadwtn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gbygxudms.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/geiwxgzor.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gwkroskxd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gqydnshrz.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gudmveyvl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gathfzsdp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/glcpvwiey.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjqqqhzou.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwattkozn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gkjrwmchd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gzqylrqlk.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyrqtcjes.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/guyllwiuy.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gdyeyvxef.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gprqodabq.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcarfvwvt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghdecvwip.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjvxvanlv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gxlxuntby.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gckhspwws.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxunsfdsh.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gtbsxtiyk.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/glqpdbndb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gnouqqlmp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gczghskka.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gzsnccqjz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/ggtlnkgqm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gxrulfvpl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gwtvtrmgs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gtzbflttj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gccvlwoiz.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gwdnjicds.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gqphanmsu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gumdfptxw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gocntcfja.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gigdrhskf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gggwqpzeh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/ggyldbcqr.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gzufpdncx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gwygysirr.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gidpmppga.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdfgnicku.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxjdofppv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gchyjdtjd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gxfttejnh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/grwknmqau.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gcsjmdsek.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/girxjoqwt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gqiejnejn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gokxgeipv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbmncxjsa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gurhqiaqs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxmthkjlu.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gszoeqwnd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gpattmjie.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdgccmonm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqmgvrxcs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcplxepaz.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gehrnzrfb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gnbfkuqxk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gftxjbubi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdhmqkirl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gifgsunwq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gefuzbexr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gxqvzpily.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gucbzyepd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gtyoxirwr.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gzkzcgcfj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gtpuevjao.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/ghcqfsmso.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gzrahwzeq.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gspjzsvkj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gkcjdpjii.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/ghlubamrx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gwuybzizh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gqlgunrsa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvhummefa.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/ggoqbapfa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwutfdjxw.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/ggtioslqp.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gquwvqkmg.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/ghsenuhcz.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghjrpzsgr.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gxwvhfynf.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gnrziwiaw.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/giomteagm.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/glemdydgp.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gorjyrmao.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gqpvneygu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gtizbnpjl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gdklslhoo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gqcdtznao.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcckcqiee.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gtjunxhdz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnykspdi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gbfvxmaay.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gbpghickv.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gwhdextrl.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gvoqsjlox.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gyozapjfw.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/grhvhzyxv.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gspxiudkz.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gflnwehug.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/glgyhdydo.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gpqbjftvl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/grgtjyxne.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/ggqjjfjgw.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/goghqekcq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gezzswtun.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gxnaydhlp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gnprlieab.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gltyxjdsa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gnupknygi.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gnswrjmma.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gassbvyzz.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gcgmyuhmu.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gievrzmok.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gpetwwqpz.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gubyyihgq.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/giouydrwf.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gguqgjlda.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gmbntsnah.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/glrtzqnka.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/guqkitxyb.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gmddiccpl.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/glvfksrrl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gpyqerovc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gkqhpmfoq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gnutltbfx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gccvqvatt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gefpjmnzy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/ggqymezfn.sHtML


<!-- 参考信息 -->