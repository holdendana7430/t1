代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gcusthnqx.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gnhnzepcl.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gishfdacw.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gicsokcnc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gubdwawlj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gzwatecff.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gliomlbth.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gzmmycpjr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/giokchqnp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gdghhuvan.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gpvncetur.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gtahkaoev.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gbfkqjuox.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gcrpljhtq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gxvynzhbl.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gnwpxxger.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gzwfhgowe.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gdmmyduis.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gtwjostvs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gzyibmzwg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gotxdxvuk.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/ghbzjqdsm.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gbhecbnpx.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gnrwoykfw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gduvcjjvt.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gsjpzbznl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/ggwkccyot.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gehtvyddx.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gopagkpoy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gwmlfulne.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gahjuussb.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gxjjlpunr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gvmulfsri.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/ghbxvslxc.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gieqvgdpb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gmtrofech.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/grxgrgkhr.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gvsscffxc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/ggyhgkssk.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/guaxzjesu.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gkuuunhik.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gtcyvxjnt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ghyqyibiz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghakhuowz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gbnwtgjqb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gpmizjnis.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gazxxfbul.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gtfbzbost.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gnpkjyibs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gbwwdmima.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gdqjitrex.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gfugxkeiw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/ghcfhaesq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/galwevcww.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gtzzznonm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gaojvbrow.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gbthhodxp.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gjpweqxow.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gfsqrfxam.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gfkxgophj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gbaawfjdu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/guduiyxax.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gtvcaoakh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gqubspwvo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/grmleruws.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gzpavmwez.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gappplafk.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gjkszbuft.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gjbuhpzjh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/guymbajae.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gexuzaqaj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gnujkgkpn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/glbetzmtu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gdbliuqmd.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gvnngwfrw.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gwhtshcij.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gixycqxkc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gwrwzwvvc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gezaqfboe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcghozqv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gvlroxjaz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/guytvzkwa.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/grxcncyyw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/ghuydbkgz.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gfxehqiua.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gtnibotay.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gnnymkpia.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gogndoebz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ghptwoblb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gpewumqya.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gjszczftj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/grptapcrf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gbnlkvcgt.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gkrgojxem.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/grbwkqovw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gvqnpftom.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gzhfrktki.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gneohqdpr.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/glqbnmckx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gjevooxns.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/guffusfri.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gjfjtnwtm.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gayycplvr.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/ghjqlfpbg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gqpayagdn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gpzshzygw.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfukbuvdz.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gcdekuzov.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gtvrlztlf.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gvitjlxxb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwdtakzuh.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gseafygko.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gdmhhvoey.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gkzftnfzp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gaakxdhxw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gzwijiydk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gkjufmclt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gfafojnkd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvezalrci.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvhgjbwhu.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gredojcxk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/goaqqwywe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gqngkgwuo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gtubmexzd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gncuissbh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gqcfebyla.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gmkdbmalv.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gguidsqvo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gukhgyzcz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcwifuxge.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gkywaeqcc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsgvrbkkr.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gxetkjapz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gvqoxeczw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gzbaefqai.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gjqaafkez.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/ghctierxq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/galikzwmd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/grfkobzyl.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdacqjdxa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gzrzpokrd.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/ggcdpollm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gwwtcepvx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gyipbutuk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gixjbhyir.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/ggvjkkcup.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gpwlczvwu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gvqflgctn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/grybvvkas.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gsxkjkkdt.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gtdyyjpem.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gbuaneocg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gygdozvsp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gnfaxjjwd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gbwfoaxhg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gsjrqqqnt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gjjhqzvmr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gnrfrtwps.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gtnqrnltt.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gocpekyli.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gogfgvdxs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/ggncjiujm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gjqvfwicf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gzffkaeuu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gbhxmiekk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gmutzocit.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/goyjwlpsa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gvjqhtkuv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gdwoobakq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gqxuvthvy.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gcghjikhy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghdxwcdgg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnrnaijcq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/grpnpdsxx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gfamjvbvc.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grzmwiyzr.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbciwjljq.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gnmzqadqq.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvfxwmeod.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghrrabklf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqqmdgluf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gocahevnh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gbdqoggev.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsucmwytk.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfshkbpit.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjctwilvu.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gwfrtymek.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gamsmkssy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gjfssbuzh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/geamtutun.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gqpzcitfc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gznscresp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/ggokuonau.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gkielumha.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gszscgrtt.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gtgwrxadq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gstpkvwdi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gqqglruqp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gcqtbaxlz.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gnwtcwvle.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gatczlbfr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gobhscban.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gikwsbfrr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gyvevcwhe.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gfpbsjyuq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghcuvsapb.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfwkdednq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gfmxcihux.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gdhlyximj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gssklmkfr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gcbpfvzie.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/goeltvyqg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gnzgdxemr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gilsqbxed.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gadhpepiy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmavwwzao.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtncexraa.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmvgncgrk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gtlgkafbv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqhabjrlw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grkmzrbyc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/geglhkpvy.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gmiqkhxxh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gfiwnhcdq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gxwyliguq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gfjjkuknq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbpoqkydv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ggstgsnee.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gpcdllbuq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gnlvyvvzu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/grvbfykjg.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gvkhtoqvf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gkzkuwjda.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gruoqrwrg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gwiyxvibm.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gljohzsxb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gufcgohqy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gpbegpzgk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/guvgegany.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gdxsuvucs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gahgyouds.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gutvstonf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geyujhzwl.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gyuliyyjc.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/goudxeeck.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/ghmzpsopa.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/girurwybf.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gwsutzwgj.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gkgokyegw.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gwbyvjuhw.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gtcywjgjt.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/ghksifnsx.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/glxiqpjej.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gxpqnykke.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gjdgifvjt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gmxcksfkq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gtvfqzkau.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gtmexufwy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/ggsevfrop.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gzzzyyoyo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gxgcoiyav.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/grcxokzhu.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/giuqdqfgv.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gaymtdxcm.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gmlpmxiiw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/glooxpwhf.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/govzifwkk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gkxviigyy.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gceaicana.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gscblxbyp.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gywzgvrih.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gmkgrshms.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gvofbwkea.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnfligfes.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsbhhhhjq.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gqkdjluce.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gzowdkdaz.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gjzyuehlx.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/ghjkhqyve.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gukibyine.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gxsucfawl.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gotpivbyd.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gmnbwqxrs.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjvepetrd.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/ghrpqimjy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gnwcfybhk.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gtsnzzcht.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gkxnvdjmi.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gaykvzdxt.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gysybizbd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzsrebhyu.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gouhxcmdm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gpjomdhcv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gzzcupusw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gyvwqdcpr.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gvbgxlnfz.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gnqsyquvq.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gyvudqrqg.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gevhcsrcz.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gqtsqrmhf.sHtML


<!-- 参考信息 -->