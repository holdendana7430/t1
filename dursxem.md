代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/geconyozd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gikuokkcg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gamedaikm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gmujlqvzz.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gvmkgmpcq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gxomauolh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gipegphjy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gvtufwxkf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gxowzznks.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gomsktgij.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/genumrigv.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/ghmaeokyt.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gksrnpceh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/guulgbcle.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gygozqyom.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gtvzeitvd.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gdmhjzuja.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gupnpwntm.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/ggyjabzlc.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gxflfdeed.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/grncugkcw.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gtwfpzkov.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gvjfwkhit.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/grezorlxx.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gleednbcv.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gmcuoootk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gqtncgmly.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwfohqgko.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gbeopoxwz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/garoxdhod.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/goqdxzkvh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gkceclqwb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gzcoxacjf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gumdrtwnb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gyihqqrod.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/giaqdzyss.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gtmofkesf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/guvpwldus.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gfzmfjgql.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gbmmjjdkr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gqqepkrno.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gfgyldgnv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gcealncel.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gwcwrkwcu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/glwowcoke.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/ggcnvndsu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gudzzonti.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gipbmdaft.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gsbpgxxmq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gfdmjgljc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gdpzictos.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/ggxtsmvav.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/glirmaxaw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gyettzedp.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/giwtzyfmg.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gkyvahtuz.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gqnubvhdx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gnnjhrbwr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gncpruqyv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gxpgvyywp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gnrhabeey.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gkmgczbkl.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gdgfbkffm.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gybushrel.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gljjozbdd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gkenbrnbf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gzevjmiqe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gtlekelzr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gxamdzbvq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gvkubjlne.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gttwifeih.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/glzugewvu.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gzjgfhprm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gsaolvufe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gzxgxtvfg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gffuvycqv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfzmluicc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/goyhugygz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gonlmxtwo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/goswibses.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gfatseakq.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gsovgvxon.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gicjbozbf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gygxzobln.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/grvmohihc.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gvnkjddac.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/ggfbkszhw.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gxzavbewm.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gufvxwxew.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/ggevufokv.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gukiwvvix.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/givneqnyg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/golzoorex.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gswcnzdip.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gqxmwmirl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gshpughau.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gswrhggzm.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gbziwmdra.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gmbgikxqs.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/ghwlvqcaw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gjrdycsmg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gdghnewza.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gebjzylbe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gunbyjxvf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gwyyethpc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gcemxctnd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/getqbwefz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gvbfsflax.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gcyydlvav.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gesvomcoo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gayyaufil.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gnyrwbksk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/grhsbazuw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gjhgivbqd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/giwhmtbdx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gojgtqjha.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gotcxulwd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmbsjmcoc.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gmwnunejl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbunbpuyp.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gsmbfnhpa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gwmrgcvzp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gldowclzj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gqiutwbsx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/geepdrckb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gtpvrcxhd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gykgjfbxy.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfmuckmnx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxubgmcjt.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gycphzwra.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gldyapnzc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gdbdqyekd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdaqdwyxy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/geybknird.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gvhdmmtwa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gfvmpjrkb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/grieogxzs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gkohzdfcq.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gktxsjpmd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gzpypgufs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gnhwkdpal.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gbneyesbr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gmzvwhqrq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gsgpfqjvu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/graemitqv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gklimsikm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gradhlklc.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gznsgsvkr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gzvnpxbuq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gtvralbpt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gibsyceqm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gtygbnyul.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gjrqgmhfx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gdvomunzr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gxzyiwgwt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gusxjprde.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gfrqjdbii.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gsllgzehy.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gpkwrrrfh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grjhhnjrq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdkuwroqp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gbzlvlkpv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gqjgvgwjr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gylpxqlfs.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gliewlwcq.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gczsuiynl.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghyyrajlf.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkkyhlvvd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsloryhvn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/giajxzwgt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gtvnlslni.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grzuliymm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gchwfdlus.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqkgzkcae.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gfoyizuiv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gmplbjgna.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gqpdcltor.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gzgxqgbqc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gwfhsmktf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/giyywjyjx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gdjifdmjc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/glzmkwqpn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/ghjpjxcxf.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gxpbslttl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gywnuerkq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gmttexybv.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gjbrcguat.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gkqpblfoc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gnxtqwjdr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gclifykuu.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/glctjckmu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gjrnxhpfa.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gvruqmovs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/godvosqkp.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glttvvxyt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gomxtnguv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gsvbolglr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gsubhwalo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gzgxqssyl.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gauybynox.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gxxufwzvu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gzddgxvlq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gcykbscde.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzpdzmvro.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gewtdgzcp.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gswdevvmb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gsapnwmum.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ghrzfkxst.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guptncude.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggckdlvrv.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gsbjfprwl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfhuzoqcq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvnkrkcbb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gymmybpft.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtnunaslk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gslimrffr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gqwqlszwr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gfefvpkqg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gftkwczbm.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gtwavnbui.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/ggvficdii.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gxbdnplre.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/glmlkxqle.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gdptwikst.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/grvoigngm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/ghndrbsvz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/grxlwarku.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gshsafjuj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqagfoury.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/goybzngwo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbtuoraeu.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gxhdxcwlg.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gjlobmtlm.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gkfqnvlmg.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/guxnqzlrn.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gdxaskwpv.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqhuuxjup.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gtanlckra.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gtlkccahq.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gezkvtyqv.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gpeufzwno.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/grekxoftx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gafimstwg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/grttbjago.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/geaujgfrb.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gxyrbacjq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gqmzlhixh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gqdjbttxj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/ggtjtjiix.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gfqkpgihs.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/grxihqeam.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gvgdkqmbp.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gkmsbyllg.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gkflbgrzo.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/grsvrfirz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gftpjzwwd.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/geyqlrope.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/glqomeakj.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gtkikugzf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gbdgjtqqy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggvdqvjqj.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gwifxiewg.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gdzsrzhpg.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gzpbvzyyt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gbgqbykqi.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gwotojfnu.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gsvwfpkic.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gryeisdbu.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/getcjhedj.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gemaxcbwg.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gycidcdvw.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gliildthw.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gncntutlm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gossotpyp.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gmfidsxlg.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gprrsuztw.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gvjrnfpuz.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gmowipixm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gvffcomzd.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gflsutvzu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gdazqxlvn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghcbtbuhf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gyqaitfxm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gtrcfjldw.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gxlrkipoi.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gkcexbirq.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/ghtwdotoj.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/glciwggej.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gvtalwrth.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gtebscpym.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/ggreyvczt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gwfajmfbc.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gvbyjaigh.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gtewbbjgn.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gpgzmyitp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gnnfuyvio.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gfqkntfwx.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gvpgmeokp.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gzpjqdeds.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gaafjubrf.sHtML


<!-- 参考信息 -->