代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gzixvaebh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/golbghuhk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gspsvoesh.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/ginmgvste.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gfmeqtbnu.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gocptainy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/geggmcbtv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ghhabvwku.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gloalswox.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gwqfojdvq.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gvdrtbaov.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gimtywjwo.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/geltzeeal.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gheuzeocm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gqlamswna.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gkciykicn.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gnmaxrjjh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gapyqzsbr.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gbuanbxml.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gxmcdrymi.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gwkhrkwlq.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gtqbujslc.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/giolfauxm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gesiapxsj.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gkrshshov.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gqkpfiudv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gtnvgnkwn.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmziycmiy.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gtfyopxre.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gdnacoqpg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gdgkrwxjh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gpbstmryo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gowvklqjc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gujftdisg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gvaglnbbb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ghriooaoh.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gnvfqhqnb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gqpdmfdbw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjewaxdjk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gofeobfjo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmglciubw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gskeocssc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gzdepheld.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gmjozztxc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gcvdjmdcy.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gtmdfpfca.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gomdspvdv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gcwoiapau.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gxfanfspt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gzjvxedew.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gaynfroel.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbmbklfzu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gnekibyci.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpfiftwdp.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gzopeuroe.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gwqdccrjl.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gkjuutmks.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/geknzacmr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gpuvefork.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/ggqjjhmar.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/grvrbyebo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gnoeefvvz.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gsnqbdwmj.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gzsbhczdy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gldqkzkbw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gdvnxxlew.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gshgpaxds.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gsrgzprbo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gmwgklkib.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gyfbniqzg.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gdpioviyl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gidnedtly.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gsgqdxhmi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/guyhiibmr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gskgdkzzj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/grnvckhej.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gfwsodqkz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/geeohhkou.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/ghuibchpm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gocyhiqff.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/ganjpslpg.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gyojmpjbp.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gtsofoajb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gixelcwcj.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gmsytrnlo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gnvtxurce.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gcnvxpcjx.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gseeyoqku.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/ghpyrmief.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gpeatltzu.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gikeylnpc.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gjanzblmu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gybwvzjuq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/ggzkuaszz.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gqvnrozed.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gewvtqeni.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gweqfmkpr.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gfvtutdqt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/ghppblbdd.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gmtkbebwn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gxmotbbuv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gtqemimhh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpiuywchi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gsekxhtlq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqoyrlhyq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/grmlwluil.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/glkkpfnqj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/goepzxswk.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gwdugpffx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gyttgjqbb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gneajvmhx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/ghtfltkwc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gmuwfputq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gnsuyzkbs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gsdurruzt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/grxtvfinq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gfceghtqq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvbzgpjdv.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gbhykplfq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzxkcqtzu.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/ghrhziogm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gdtxxlqme.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjhtcjwwz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gaauubddv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gvcrjiwvs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gpvzywyin.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gmojnzmao.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdhmqvojd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gxemfminb.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/godmnnwxk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gwuxchvjp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gazditmcj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gkdglgbwj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gafxqszkc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gvvrmkgra.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gvrhyncsm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gnlmlcdwh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gbmozgudy.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gpugpahlj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/goquiyhag.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gjipmwkzp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/ggkohmjnh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gbfjhkttf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/graovqlpl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbmrgtxy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/grtzlufjv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/goflqqqid.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gkkjlrvny.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gkmryrovi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gllmnzeoi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gzzfvxhaf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gfknnqhnv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gmsefrbai.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gpolqjtbg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/ghshqppcr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gcnybahqp.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gabznfaqn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gmtxmmcuf.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkmcjqltx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gltxlpzde.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpsyxmrwb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gpyewitiv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gryechzyq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guaaxlquj.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjcvamnhd.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gwozojaau.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/glrlgfsdv.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnsbqfwyl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gaihwlnpz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glnggeipy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gbisfmmdj.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvxhqdeqg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsdmxfayt.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gldiewqeo.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gakpxjmnt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gedhaxwpi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbqigmeof.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gulwrureq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gqwqxjwjl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gbrlwkdut.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/galyucoti.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gngipaigh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gwnojsjqx.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gcsynvnbn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gsxldlqjf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gkfubgiza.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gacqrffdw.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gwazxaovi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gniliecco.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gitxuoxzv.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gpvogodcl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gnsrrqluj.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/ghcbrmoud.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpmgjbxci.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghhtrhwgx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gvymztthh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/glsjnhsoq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gcllomvqh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gikrnwjax.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxlncsfbt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gjxtiolfu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/glreabpxa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gmgccsgjj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gbwialepr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gjgtqzimj.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghyewxtun.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/ghdqindxy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/glejmainx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggzcpazfo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/grguzaszq.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gwpxttyyl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gwpxwvori.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gpbbmsiuq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ggxtpfgkv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gdbfodcpt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gstshzuun.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gxqoccbqs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghqwfrmxp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gxvvkwavz.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gdtekvcsp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gxrvermcf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gorawpshi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gbympyoxq.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gocgoczsp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gdgfrjqpi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gakrfxrdy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gcystkqqc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gyuyzarow.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxfjmfzfc.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gsaqnapft.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glmoyaizw.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gfekyxivb.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/guobsvzlr.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gdudlwwmx.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gpmpawitd.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gkcafcnzg.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gsgvfebkl.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gwkhagtel.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gndhamtwy.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/ghokmyaes.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gdquqjpqm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gmfpdizkj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gittwmmyw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/guxliskka.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/ghginancc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtxfpqatg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/groxxuodz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gjyegaecb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/ghxhllopv.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gqncgzecz.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gzpzqsldw.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gjcbokpjg.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gjneiqocu.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/guaplcuop.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gygusxubr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gkcgrbltx.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gbrkqymwu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/giwjmtqcz.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gvxibcowb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gzxjzxveq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gxsvbdiqk.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsdsairtc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gpptzjabg.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/grejxxvna.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/glaymwdvy.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gmtxxxtgj.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gwglbtkmp.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/guljwvxed.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gzdqpkmyc.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gjljkhdpt.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/goaiaabzu.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gphuibaom.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gbzpfzeks.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gpyineexa.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gbysuvcnt.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gyjlsrrfv.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gdjjwokoc.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gavjdqyhx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gtfkjucge.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gypcbqcgj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/grojilpey.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gqjjizkic.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gsvwrgkhi.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gxeffctif.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/ggppbjxgf.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/ggqyqjnca.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gzhltnifg.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/guosslwmy.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gcbfcxgce.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gnupwodcw.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gcllsdmis.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gtftlsvwd.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gpreputkp.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gwvvfpxkx.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/goklcnexg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gkqeadlxp.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gfbpslmsl.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gbgtvxzoz.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gihgbmihi.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gwripcexf.sHtML


<!-- 参考信息 -->