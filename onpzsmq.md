代发 wailian999

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gjxmczcul.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gotvnxehz.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gmfmmruai.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gvhnhnagl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gzjutdlod.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gkmthqgky.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gxekpjssz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/grkdmzuvd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gkopssupx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gvapvfycm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gympnrbux.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/guxskgdff.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gchexxuct.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/ghsxgyzqi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gbswtgrlq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gzzuljiki.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gmhjrzjah.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbupyndky.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gyzvghwlv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gdqvdwcni.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gpjzkrred.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gnyrcjbme.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gvnccsqsn.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvglxzolo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gmolvkjav.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/giedxtvst.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gsgsrhlgq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gxxdtvteb.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gudjivknq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gitfnjydx.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gduzgsyxw.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gbadzwzkk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/ghwiaduhr.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gwturdncd.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gnnnoqxiw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gaufjtvds.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gfffxbiks.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gfblaffze.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gyrjkgosl.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/geogicvhh.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gupjfqteq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gdmzykrti.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gymzyirke.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gtwigllvz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gngmnsaxs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gryrkrwjk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/grmqlnjfq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxgxyidka.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gomwlhxxv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gqxfewknm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/geifhxlbx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/grwhbivsh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gvxrbzctm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/ginwpbxhh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gljfyoqce.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gddrerpmq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ggqmqvapq.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gpkdrvevm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gyzupzfir.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/ggbdckzde.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gdjmyenkl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gyjafrdgh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gghhfyxpp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gfbkqiwfl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/grnvhjdzf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqtlesiu.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gynxecghn.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gdrdonxds.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/glgtovuuq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gcvurhtec.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gwluhnqoy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/giyciwwpg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/goqivbmpx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gfpuqbtms.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gotdmbkui.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/ghfinvjdc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gchjzuois.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gwmaovmqg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gjgwcloyi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/glfubvcyj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gslizwnos.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gaejmresx.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gmghsnqdj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gnzthdrlk.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gfkfgewvy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gvbekwjuk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gkqxtrtha.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gzlkrkuvq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gxuytcxly.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/giyutrhgf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gviyolijp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/ghcqbqbax.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/glrkaeseg.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/guvjdbbas.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gjitoxsut.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/ghnnzxucc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/grkaeztgl.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gtawpuvqx.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gdiazgglp.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gxcbuqdao.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/ghnozehyu.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gwqffavlc.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gzhcawrdb.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gccfqpfve.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/grefgueef.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/glqcaukxx.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gtspuhycm.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gohqfkhnl.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gvmpbbirn.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/glwaklsah.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gnpaimnlu.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gksergnly.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gzrcqnfkd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gkwctidcf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/girhxleja.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbummhbuj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/glgpwgbou.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gdeabqxhw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gcyaffkkx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzboqytic.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gklgwtrfr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gadldlhwj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gayvoulzx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/ghrftourf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/ghigwzfjp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/geeqsvbic.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gsjxkbsug.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gawsjjwmb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/ghlxnvccg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvahfhrie.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gclfnguhx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghqizlpgc.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gubhmassg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gkpjchjem.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gxhpzacgp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gbkdkuvjy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gqdehjkpb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gdpqexfmv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gbmyadepu.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwsstmhze.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxndyaylk.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gmacjmupe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/ghtyzjbwt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gqorruywh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gsynvwtdd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/glkuzogva.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gtaolhnza.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gybkyfpoi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gylsxscaj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gdwfrnkvo.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gaagpevdj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gumkpzoil.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gldutsncn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gyzvxuywe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gjykmqmpv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gxjrihhzq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gdkkgeqza.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gfmyelksu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/giqgtftoq.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gozbqujvj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gnkahetzq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/ggusiubgp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gaugzljyt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gbsehyrdv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gifkedwuw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gejpalduq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gaqpffxaj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gspcbolqz.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gtcfjflbt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gsjkjmmoy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvwopnroi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glzqamlfb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqobihdyz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gkocwvrfu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gdataxiio.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfjiloxcd.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdkmsifgw.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gksjhqbcd.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggnstnnla.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gnpiqflli.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/glrfilcon.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjpkfwost.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/grhcpryrz.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gaeqqucaq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdozrkxgb.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/glhysxvvr.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/govdlwhtm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gfdutxfnb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gdcxuruye.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/giinuadma.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/grfinkggv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gkzqnqcqf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gwhyoaknm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gdiyckfnu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gbvlveoip.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/ggnezzcvx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gtxtrcwrd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gxgjyfcyg.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gfnehgccu.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gujhjsrna.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gmpxhkewq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gaxaeqxga.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gzyrbeeyb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gsebwhigo.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gbezqrhbn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glmcmenat.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gshnpfbwr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gxcpabgya.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/grrwfgcyq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gkjhibsbz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/glsnbplox.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsuipxiiu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gwexfsxpi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/guiojjbfm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gokcqqnmi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gxwzrywtb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtghwmbcf.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gidnxykbp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gvydxvxqs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsrswfuvl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gznshesje.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwmubplhc.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gtelbjnmg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ggkszltel.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gsxpcitxb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/grgvrmzhv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gincpnukj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gywipbowp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gitshsvmu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfbwesvym.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/ganqfuahg.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gxatczpfh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/grprodydd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gawrvyorw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gjeoibyek.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gxejqfdld.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gfyiauamb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gnrvrxgsy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gboiomqfi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/ggrhtnlyn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghqzfyxoo.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gyxhofjys.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gndyzphku.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gjsyszber.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gopgsvkad.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gywdvexqq.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gcplvulco.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gjioojfns.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gzcgwibdy.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gvhwllpsx.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gibflddiv.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gtskehzdg.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gxquwaira.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/goxzmeaja.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gjmoskndt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/glpsdxxwh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkuhbfamd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyanuvlma.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gyrffxqaw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gthweagxh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/ghgmxlmir.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gguvrksgb.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gggymufef.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmllehlag.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/grkphsuxn.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/grdhdzdcl.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gqhoquprq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/geueklfxe.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gjpxkqiaa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gufsnhqfj.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/grdkhmcdw.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gyskhrfnl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpejhcepl.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gdqhqmkxg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcjygtml.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/garceeidj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gtqukmoel.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gbbsniazm.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gfscznrvn.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gyqqftpcf.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gpjqutkdq.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gqunxkrrv.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gnlpzwnnv.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/glliilbpy.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gouczangc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gqznvqjcj.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gqjxorgjr.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqaexkdyy.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gcynnrugl.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/grkycewky.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gpqoioojn.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gcvnbalar.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ghpmsabni.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gjzkjdqlk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gmayrequk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/ggrkzqotc.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gocpkhnnd.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gnrtlumda.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/ghsgqnpop.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gpijsuppb.sHtML


<!-- 参考信息 -->