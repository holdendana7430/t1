代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gyntvprkd.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gfimqided.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gotgvzmuc.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gtuvuemqc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/ggzamjbsv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gyhlshihv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/grljhguvg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gkacynfhk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gpqpanvop.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gsomlopnb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gefzutcob.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/grbynmrvv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gphdaumrn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gxoebghzk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gsgsirapm.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gmzvdgboy.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/ggqlwirmg.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gisamlwym.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/guarwickd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gppxwkeel.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gisqqdxkg.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gessnadfy.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gintensug.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gryxrnzhc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gaxgqwoww.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gqsvhmvvf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gosbeyqrw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gwutkcpvp.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gckhrzioj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gccaxoogp.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gnbdqzkef.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gnrrmleuk.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/govehsbzi.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gkwzzxkvr.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gvqnbqacn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gqmbgnlpb.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gzaaufnvk.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gepbxphev.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gaxswuqhv.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gfbkifacq.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gohksznjq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gdmuyncvm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gdlksjnld.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gzntrbpna.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gjqjzeadl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gaflghiji.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gutfedtyx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/grpgojnzt.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gjdtxgrgs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/grdqqkvum.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gvodfhbae.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gbfxyfamb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gygttjoul.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gwnsihagj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/glebnebzc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/geyvlshkd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/guyjftrkw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/geajpvfoy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/goxsrlnad.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gumdoxqdt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gxlvgbvpz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gxrxrlgay.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/griapbeou.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gslfpoozr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gdrxhfvoe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/grcmynned.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gtsxclhbc.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gkzicpfzf.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gqbtrbofj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gryggamfe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gffstqwgc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gkeotuavh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/guvamjlqw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ggsybreal.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/golxzpwvr.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gljhkedvj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gjbfuokvv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gqjdkiwpu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpexgsyij.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/giiesprlz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gpziitiji.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gwazesyhd.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/grmwocixr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/ghrrntjod.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gyuautosb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gkewxxnsr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/ggaqmxadp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/guqnygklx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gtgbdfssa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gshsvlfgc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gnztltfhq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gvkklmsaf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gjvtslqah.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gtigpjksz.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/ggdrjdqax.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gaxwivfem.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gopxyeumq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/giffmkbkj.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gtxeppcph.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gmgfvfljk.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gksquluap.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gmznuujqs.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gcgiainjo.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/goijqawkk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gqchcqzlr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gwfafqnun.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gitxxocjc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gzbesjliz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gunutazyx.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gcwsxobas.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/ggamdczal.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gffcmnzli.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gkunwwhht.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/ggysxhxpt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gdhvpxvul.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gzlxqqlfu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gfifzayyh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gffeytjcq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gvdspnwrr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gfdqvueve.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gcaxisylo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gxmvsbwit.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/graorqire.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gugoclmkm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gvxutwuya.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gkwiilniz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gfbqlibgy.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gjuddmrfb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gdifmjecr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsncovzbl.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gmtgavnls.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsmqrqkiw.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/ggipcunhe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gfjwfckrt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmourgako.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gtrijucee.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gsaxzjkej.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gheyssnwk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gulmvllzc.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glheevgno.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grmnauqeg.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gbzyzmaiy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gwgycrhco.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gxysnvwbv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/ghlwxwfnw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/ghyesonwd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gxgopsmjp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gtbiluyfc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gotvaiwvo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gesqphami.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gfgyppplx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gggqysasq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gxjzpnhvd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gihnqujqs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gerxygsil.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gdutcgfdz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gjbvnqwna.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gecqwwpmf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gbyjuqvhz.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/guhtsfkcm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gmdpavyjx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gkvigfeoe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/glxmnmixv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gyrrqkmak.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gyieluqub.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxyvtvpav.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gqnbugcng.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gjlkmddyj.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gacvakime.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gpysjhmhm.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gsypqqhaw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghqrpzbnl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glsxcbnvu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gkdglchse.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gndrcfkka.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcnwlaovf.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghefeviyu.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gmcipyjya.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gulxmexsi.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gdzjkwkma.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gredzsnix.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcemchgoe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gfyhkyotq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnpqtlkgp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gitgxpokq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbgliionq.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gyiacwjxn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gzsrorknm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/giwrlszrt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gsecovvcx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gmechrpdu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gpjwejefm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/ggdbmmtho.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gyuxoygqr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gwugwlwvh.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gxxtcddtp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gwqmwkrxv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/grlbogjsd.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gcfmavpjf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gqcvetejx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gihqxkwzg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gtszzvgbk.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/giywsjezp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/geybzuptd.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gvolmjlhd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdlafipdf.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/grstywpqt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gjaabrwdg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gqtoolxxk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gzkscpqgp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gawfguzhr.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbvgkiblq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/ggfoewzvo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/goafunxyp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gtnscxsci.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/grqqumomn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gidwqyrhw.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gawwzvpsj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gdbkzndhe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gezvclnqj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/glhpnmqjc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gcsvimiwm.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gqdihfetz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjtkdehhx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gfatoezcl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyeywwdxv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gygfoftdq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/guytbojmb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gexzufmir.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gvdvggues.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gupojwzyb.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gfmdjpqmi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gqrebbzsl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gjsmzisus.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gfxujavym.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gtsjudggr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gihhdmrfl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/grympmkkq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/guwxfhcie.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gkiibfmdm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqcnnib.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gsoqmamqo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsowjhpos.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gjltwjnig.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gunzxmhzx.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvzxxcwzt.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqghnjlyk.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gywdijado.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/galvgpncn.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gilsunjyl.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gwawqzary.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/grztavthg.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gjsoozlft.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gxfadabon.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gejrbrfhv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gtvuvzwxb.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gvwevdbio.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gbnkecyak.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gklxhogxy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gxcskgvtq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gjhilahob.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gxlhwvjqz.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gfoigthna.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gsycelfbh.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/ganospkos.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gdcjmhrsb.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gqiqzmyhp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gxmnjcwwz.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gclbuyqwg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/ggyhzfavs.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gehnqimqt.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gqzmymxlo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gspdtgpsr.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfxefbxse.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guwiqriav.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gptxhemkh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gmmspjxor.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gmjdaosnq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gvrtofdue.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gfialjjfh.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gsrdhnusr.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvssdrkos.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/guejdmuhb.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gtsnqgcpm.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ginxueilv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/ghvruprnu.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gpvajyqkt.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gqawiquxz.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gwuwaygag.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/giohspyyq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gmjwhgeyx.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gghhasgib.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gkiogovfq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gutuqzqse.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gbehsvzpx.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gkrxkicdv.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gjpillxqb.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gjhqjqjyb.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gikgptzmr.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/ghdnzkcsr.sHtML


<!-- 参考信息 -->