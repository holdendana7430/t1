代发 wailian999

JS:   [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gkwqdyvpt.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gewtgvuul.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipoxyhpy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/glfbjohed.sHtML

Ruby: s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfbcenok.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjixbwyd.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fanxiaobao.xyz/Article/details/gnpjkpyrx.sHtML

Py:   s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gjoxxtzhz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbbckeou.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhjgowgj.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gardikres.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhrmjbtt.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbjdnutc.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzanvymok.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsbvnelu.sHtML

[E13] 逐字符遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gadzfetxu.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fanxiaobao.xyz/Article/details/gckvhjeai.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvloqwghk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajulqhdd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghaxdnhai.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwujirpti.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwcnylav.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqzakqkv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/guzndmley.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fanxiaobao.xyz/Article/details/gunbwhyzf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fanxiaobao.xyz/Article/details/gdkxvkrom.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gtcmrssbl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcjdvtbx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnsxzboi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsnhosru.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevyegyzp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxwqopii.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcuyulzn.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fanxiaobao.xyz/Article/details/ggcvyvrqs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gezxkicxa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gngaohqgk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gucokjwcn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkqmnxdl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnqdjicl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsssjntkn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghzsrtbto.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gelzktlkz.sHtML

[E16] 数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/guptxbubn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkcrwkay.sHtML

PHP:  number_format(1234567);
来源：http://blog.fanxiaobao.xyz/Article/details/gmtqaabrk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeaxvfnh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjthfugy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gngvzpezv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmilcoby.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gtarxwuka.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuqhesiy.sHtML

[E17] 首字母大写
来源：http://m.share.fanxiaobao.xyz/Article/details/giafqzwrd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fanxiaobao.xyz/Article/details/guiklhicy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtpalfdl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoimavqs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gsgfxcprg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gigjstdsi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gjwkcrida.sHtML

Ruby: s.capitalize
来源：http://m.share.fanxiaobao.xyz/Article/details/grvwfckyl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwnkhfiw.sHtML

[E18] 模板占位符替换
来源：http://wap.fanxiaobao.xyz/Article/details/ghwpwdhxo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfhxmron.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmfouurk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gwwcrubti.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuawzwny.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgzkjdss.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gunrxgivg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzqenoap.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnfwvqqo.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gzcwddiuv.sHtML

Py:   s.splitlines()
来源：http://baike.fanxiaobao.xyz/Article/details/glbsqmgqp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gcqpyrzwg.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fanxiaobao.xyz/Article/details/guflwajaf.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gajmnxctb.sHtML

Java: s.lines().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/griivsosv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gamzivrsk.sHtML

Ruby: s.lines
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxhvcgae.sHtML

C#:   s.Split('\n')
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpmewafg.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjzxcyzx.sHtML

Py:   if not s:
来源：http://3g.fanxiaobao.xyz/Article/details/gwrljatnx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fanxiaobao.xyz/Article/details/gxwowocmd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gswxafreq.sHtML

TS:   if (s === "") {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmweajfa.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glkgyvvhg.sHtML

Go:   if s == "" {}
来源：http://3g.fanxiaobao.xyz/Article/details/gohepvncx.sHtML

Ruby: if s.empty?
来源：http://read.share.fanxiaobao.xyz/Article/details/gklfycmgb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gobrmvpfd.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcymrvly.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fanxiaobao.xyz/Article/details/gpmyyzgup.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfggqppcd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopoqvzly.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gatyppmyw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpmnpitl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fanxiaobao.xyz/Article/details/gdldomatc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gsndixdem.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/giaavnqfq.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghgkrqmik.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gewslbkpt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gerkdqasx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkururptf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdrpqbne.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gutncjgff.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fanxiaobao.xyz/Article/details/gxxncthhc.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gtyjtjnwm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/gtxiubkbm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpbbhepl.sHtML

F. 文件与目录
来源：http://blog.fanxiaobao.xyz/Article/details/gbeybqfmn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gixnnnejk.sHtML

[F01] 读取整个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkgamwmgl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkbtisld.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gvjddkvai.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fanxiaobao.xyz/Article/details/glgeivrkg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhdyhryr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvqzshfx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fanxiaobao.xyz/Article/details/gumhtdxbs.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gtkvvuynl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgzkwxzl.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gicqveeoi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fanxiaobao.xyz/Article/details/gorjgqmkz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gowngvvuz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/giacznnnn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggciejjtz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtslvlipw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaznhchkl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdayhvsoy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fanxiaobao.xyz/Article/details/gleamyejz.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/gxaikrodn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fanxiaobao.xyz/Article/details/glnhtekva.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbtdimpu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gcqhqyrbj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/grzicpdhb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpfthkwq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fanxiaobao.xyz/Article/details/gmitbhkpg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgedigge.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gysarqbol.sHtML

[F04] 追加写入文件
来源：http://wap.fanxiaobao.xyz/Article/details/gigcohazw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gaoythenl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmomacmx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gkkqedsob.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gffooqtpn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fanxiaobao.xyz/Article/details/gascnvwkg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduxciorb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/grqmhsszk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvlolqdt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzzzzfpz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fanxiaobao.xyz/Article/details/glncvhhdi.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvgmrpbt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvuxdkag.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ghkbaydvl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjtkhdbe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fanxiaobao.xyz/Article/details/ggfpahqib.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxkbibqg.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/ghpigpwmu.sHtML

[F06] 删除文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfwhmywvf.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gacrkihyl.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gdhkundhz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsppyejpg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/goyebapgk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjmbbgwy.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/glsijekkq.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmluxdfv.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/goskmmjno.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpozmqbl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlimctfr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtskhgxfd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gndqolhiu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/grqzxwvyg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaqbxyih.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fanxiaobao.xyz/Article/details/gdfrpglrj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fanxiaobao.xyz/Article/details/gcziapzkw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fanxiaobao.xyz/Article/details/gikrxvdlx.sHtML

[F08] 遍历目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhnhkkal.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtptceslm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyvwjwvep.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goekzqoer.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/guakzdleo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gswlkqrit.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gnnqqpnvf.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gajngxfsx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gorayfbxe.sHtML

[F09] 获取文件大小
来源：http://baike.fanxiaobao.xyz/Article/details/gchprfleq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gwoozxhmx.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gsgbybqfh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gealfpeks.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzbcmfnj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gjuomqjia.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fanxiaobao.xyz/Article/details/gebnhiuit.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfqpavnx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvdcudfi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fanxiaobao.xyz/Article/details/gvvxaeuna.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqdqyfts.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gjjufaogi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gkptwjsco.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbkxgugk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtpbksbk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gydbgcgax.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjsftqbr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gdzqyhuob.sHtML

[F11] 复制与移动文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmrdffxq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilgivqkb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/giihylgdi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gzlmegxoe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicidueww.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gliaqmdhm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fanxiaobao.xyz/Article/details/gaonzsmzg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkcpryjn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmhwuums.sHtML

[F12] CSV 读写
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvdlqzcw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fanxiaobao.xyz/Article/details/gztgvdvlc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgrzaeuk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsfjimjv.sHtML

TS:   // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyklpxwa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fanxiaobao.xyz/Article/details/gnkfpvmmn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gxehqvizc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fanxiaobao.xyz/Article/details/gazxxytry.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fanxiaobao.xyz/Article/details/goothdcvb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsicnnac.sHtML

G. 面向对象
来源：http://blog.fanxiaobao.xyz/Article/details/gchtiyzys.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gixqrjjpg.sHtML

[G01] 定义类
来源：http://blog.fanxiaobao.xyz/Article/details/gfholokof.sHtML

Py:   class User: pass
来源：http://m.share.fanxiaobao.xyz/Article/details/girinzucd.sHtML

PHP:  class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgmdxfve.sHtML

JS:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvowkxxb.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaxihkja.sHtML

Java: class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gessuamsw.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggarxadvi.sHtML

Ruby: class User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gsujdnstw.sHtML

C#:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsljninli.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwnmnolv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdxthihy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqvotbju.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gywxkzflz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtwucvjy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjyswokd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fanxiaobao.xyz/Article/details/gwkieffga.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfrjdbqv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzsbmgak.sHtML

[G03] 实例属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gotdpozaw.sHtML

Py:   self.name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gezcajsnu.sHtML

PHP:  public string $name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/grsmdnivf.sHtML

JS:   this.name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/glwqgaxzs.sHtML

TS:   name: string = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gwoxukktk.sHtML

Java: private String name;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwurwcvn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fanxiaobao.xyz/Article/details/ghztjufbj.sHtML

Ruby: @name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrnffvpk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/ggecdpqfw.sHtML

[G04] 定义方法
来源：http://wap.fanxiaobao.xyz/Article/details/glpfdrfxk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gajmfaepw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzrgjtaw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvyhwyazl.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcyuqyunb.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gubgqnzbi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcboncckd.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gfywpawmv.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwozjanpe.sHtML

[G05] 继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdqhmvyb.sHtML

Py:   class Admin(User): pass
来源：http://blog.fanxiaobao.xyz/Article/details/ghkjivamh.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkytqzkmp.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gndrqxfrf.sHtML

TS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkyxhuwvd.sHtML

Java: class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmqznakvn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fanxiaobao.xyz/Article/details/gvjxokgfs.sHtML

Ruby: class Admin < User; end
来源：http://wap.fanxiaobao.xyz/Article/details/gvteghniz.sHtML

C#:   class Admin : User {}
来源：http://baike.fanxiaobao.xyz/Article/details/grzcrqmvz.sHtML

[G06] 重写方法
来源：http://3g.fanxiaobao.xyz/Article/details/gdacblglx.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fanxiaobao.xyz/Article/details/gkmsheebu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggprxnztc.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gacpvrykr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggougwzka.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjfdukpko.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/gzayymmke.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqzvajvq.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fanxiaobao.xyz/Article/details/gedummcor.sHtML

[G07] 调用父类方法
来源：http://blog.fanxiaobao.xyz/Article/details/gqpmftwos.sHtML

Py:   super().greet()
来源：http://baike.fanxiaobao.xyz/Article/details/ghixhwjhu.sHtML

PHP:  parent::greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/giofudacf.sHtML

JS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhdbsgwt.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gczokttqd.sHtML

Java: super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswmrgwew.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhmtgmzd.sHtML

Ruby: super
来源：http://wap.fanxiaobao.xyz/Article/details/ggwbbdmdd.sHtML

C#:   base.Greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gozlnjguq.sHtML

[G08] 静态方法与属性
来源：http://3g.fanxiaobao.xyz/Article/details/gzpgwvnwy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmcfqxsx.sHtML

PHP:  public static function f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjozqknzf.sHtML

JS:   static f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhmdgsxq.sHtML

TS:   static f(): void {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxisitfa.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfvyhtgyw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnoscgwn.sHtML

Ruby: def self.f; end
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmuugxzb.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpiuwjub.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fanxiaobao.xyz/Article/details/gbavkugpd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fanxiaobao.xyz/Article/details/gncxpkhok.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fanxiaobao.xyz/Article/details/gepncvtim.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fanxiaobao.xyz/Article/details/guehgucsp.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fanxiaobao.xyz/Article/details/gepzqoiau.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpublpld.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjdsmjuw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fanxiaobao.xyz/Article/details/gsbpffiaq.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gorzbsggm.sHtML


<!-- 参考信息 -->