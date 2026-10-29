代发 wailian999

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gkasuthqx.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gjdgewbpb.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gmyuxugsu.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gqsgdfdeq.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gxzimbgyi.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/geljsrtfy.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gjtudydbv.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gbdpixjsl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gnonudaoj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/ggwcigzbb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gakosyycs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/guwugftql.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gzrlpatvq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gecscneks.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gkodhzbpl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gubtngehn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gbmlzzdpd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gxqnadfso.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gqztmhovz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gpwfoyctx.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gytkoyveg.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gkmrwufye.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gisvmwklo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gxqmdbtqq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gklydfmin.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzkjzfybs.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gnksgtvus.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gxhfuhylk.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ggmrhdbrf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxocklgnf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gpoyzxmyl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gqpgrsmzz.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gwthxrxos.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gkgdpbknc.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gfklmtefv.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gujpratjv.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gylvpovya.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gqawjwscv.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/guegcdgpp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gqbabcmpu.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gyrogkepw.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/ghijqxrof.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gktwcdnwv.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gsfuwnzoq.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/grvyenzlq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmxuodaog.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gmvtrqmjp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gllyqrgyy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gpipkmlzv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gjatfqnny.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gsufldpni.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gynnmthfb.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/geuudqqwe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gcqfbagjx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gkpaxyuij.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gatgenoif.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gvsxtnbxr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/ghvufnugj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gpqrmjekc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gtxxodixv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gkmlnivwy.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/giyjbrgkl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gdbjinlvb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gdyaspozl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gojzaoxju.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gpaonesqx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/guqchyies.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/ggsqbwdvj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gdukakqkm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gerehupzc.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gjlsfojuf.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gjkahkrpz.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/glghmdjia.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gaqjndxil.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/geiocumzs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gbfuxfuxf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/geqpcxosy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gpdwcpvgh.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gxquknrca.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gfuwgysio.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gtmkywdig.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/grvmywcbd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gevquomih.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gnsjuccty.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkqkvtvbm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gtzanoupf.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gwosyorki.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gzxvkkdmu.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/ghjylbrdd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/guiaahpzg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/grfvblxpu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ggbcgotyh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gnefswciq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gpsorgkna.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gquzdmlsg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gujmcqtpw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gfohvyhcv.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/goiigubns.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gebgeqqom.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/guxhiushe.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gcijvcchf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gmqfsppsw.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gswbdufnp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gavwtcwnd.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gtejfkikm.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gokrghwar.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/ghsqlukkd.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gfvelnqgi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gvkvkytcf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gkenwvwfk.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gjmpkrayu.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gnusfrbpu.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gfgnhfugo.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gvaggryzk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gwdchinli.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gjqvheluu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gkzgdpfro.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/geuykedaf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gzvralzvp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gzfmpwwrb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gvelcxxjg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gpadsfthb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gdtgwxlsb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkmljiyjn.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/grhairroy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gnixrvwcw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gmjvsswef.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gqucgkkkr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gkfagonrj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gescyplpc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gpfszlrbq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gvpvrhkqv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gwozjoupj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaxtdwkpt.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gdcvmlevv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqvotjlqi.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gwkupnkxb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gwuipbzew.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gkasovvfw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gwscrawai.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gdxcqombf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gqaxircrd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gvzjnlzdf.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grirubzvu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gldiekqav.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/glohhechw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gvnypbmgh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gvsvnwzio.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/grobwdseg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/giziazaro.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gnbsnltyy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gufinafjn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/givdmofmg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gqsfcjejx.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gzpzxcxge.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gebcswrya.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gxqnqvxzt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gmtfscumc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gnvetjqgx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/guueocyfb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gmdnzziyp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gcbowwgjw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gwhzgslrc.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gqxvczmji.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gdlnablgt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gjukthcie.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gybsslezv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gwgdtqwrd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gdnawrqkx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gnmsdqtaq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gzfyqwsld.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gqycnzffw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gnmcwmpzb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gudgxdkwh.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/giycfdavz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsgmitybi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbgnyuisr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gjhtbxeqa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gkzxzqgxy.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/guekbsmbb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpsabcpuf.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gkkjutzee.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfmrbxhon.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/guomfaafj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gujeygtmg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnsklfnnb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gavvzbjqw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfxkwexfp.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/grqcjpndf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/geqfadpww.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/ghhtujgyp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gwnzdgwzv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gxfxxvjnh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gnqhijlqk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gtrljejex.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gilhjxsnd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gdkqaugtk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gxzsvuxxn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gllrzoatg.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gzbnjemsi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gcgygxmqr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gyndurepe.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/ggculykbc.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/giydbawhe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gcaxircmt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gctqfwrhz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gurkwajzu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gerkixxyo.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/grzfgaitm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxijwqthw.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/grpkaomop.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gamuufjwr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gtfmyorcp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gbyrtpynz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gpnlmshhi.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsbryqvvs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gdeocryjk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gsvucwxbe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glinndhqf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gbvcbzylx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkofotxax.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtaahwznj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gcuatxqbm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmaoisgbq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glavsxgki.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gnxdunjyg.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gcynbszzl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gbkhkeyil.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/geyuvfczb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gldeeloej.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gpsodkiic.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gznhsfiof.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gnaeffjfc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gxswbclqi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdazvjkt.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gyijmpnkg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gejrgpnoi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gkdbtnysq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gljkvndee.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/ghkzgovyh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gwkbrzgpx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gmragcbyc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gwwjlbnss.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/guwljpyjn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gynxuujow.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/ghdnmxbjg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gebrtjwrr.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/giqhxsmrq.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gplwnlpkp.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkjlfnale.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvufqdcoo.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gyxtkemer.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gunwtssbk.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gpvhyrmov.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gbrulswen.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gsqfbmjid.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gmabpxdry.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/geisullas.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/goclbzmnt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gfkhpfosa.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gdpjaiayp.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gjdbbryet.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gqrivzmhi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gndffvnyt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gusjnvrhr.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/guceemowd.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gjxxcixdf.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gszzmucug.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gacdfzprm.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/glpqsvkbo.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gfsdcannp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gbgwrtcct.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gstfmguda.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gzaohldeg.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/ggovevnry.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gdcsmfaml.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/glvgxbtpq.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/grbpwwngu.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ggpvdspse.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gkdafmctx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gbgggnske.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gyvslspgt.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/ggdzvvezx.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gwrrdwfjz.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gppdrfclq.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gffbtenpn.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcnqwiemy.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gbwyaaolg.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjjycscuo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/guuelcxll.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gyopctdlv.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gpsgnhmnl.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gmvqfjjzn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gnipkocsy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/grujmyung.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ghvfqckow.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqcddwhmr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbejqwrsn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gmayavktv.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/goqwgsuep.sHtML


<!-- 参考信息 -->