代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gpnxxoaxc.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gaygaobtw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gycubmqrm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gqtbcuiem.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gedlncvrx.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gynmwuzsx.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gstqdfgpz.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gooqivwzi.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gjrvbrkty.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gjanygwnn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gslwbtuga.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gbhfsipti.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/ghrkenxqd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gcgagdkvy.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gulpjvryq.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gixpbhlcg.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gznpjhxdt.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gzcnhhtew.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gmveuzijy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gitbmqboh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gctodabaz.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gtuhreuob.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/ghdxnyfdd.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gfqfflfas.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gmasrnymo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gtdevqgix.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxnspoibq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyzaqwzug.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gplphhhzb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gqvdiqflf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gaszkurdk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gntizxjtr.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/ghxojnsiu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gablbfewk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gcafnuetv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gvmpfyhfw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gtzwnbmzm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gteywabyi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gegegbhln.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gathoqcgj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gmjdqpokk.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gfrnntsmx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gmyganyzk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/glqzhtyux.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/girlmsrfc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gymgtkvmc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/glflzpajj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/ghyfjixqs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/ggvnlaaha.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghiedtfni.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gyjwewahv.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gwmkcwazd.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gljiydvfs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gszpknysa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gabdzrkdo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gjawjjlbd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gydvbhiru.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gcdbksnnn.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gjxiucbhn.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gtjthpmqr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gxfhvmqdd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gzokevcqf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/grixtrbyv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gydhlvdos.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gjrrulhvt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/glbfktwps.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gucwsiupk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gabfrmxpg.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gvzrqpswi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gfdcmqoqb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gpcdajyrl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/goqfkcaaj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gofdjxcxy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gkmkfuwfs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/grrolexjx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gnkwgbrza.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gbozhqhjo.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gawgyijcj.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/grqxsvhan.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gaxkqaxus.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gdvxzvkvv.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gvnnddftj.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gkenhoksi.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gmxppgkmu.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/ggtjerxws.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gjakdhgqp.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/grmmjuuqo.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/ggmrjensf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gdovxzrnd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gggmgrnuc.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gcffrlfvu.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gzevrntxw.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gaiwlpwur.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gdoyrdsnl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/glbnnlidn.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gzfhwauua.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gxscsoxcm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gxqvxxoot.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gbrowstxw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gdhrilctn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gwqqtpawh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/grjtefbkz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gubqlqntx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gdqhlkocb.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/giaenxqis.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gnpygchis.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gswkkqlmk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gzxzvvrdk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gdstsrwen.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gvzfjtjha.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gavnpcktb.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gjawkcvmy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/ghgbicxun.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpcngsumw.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gtdqpsosa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmfkxczqe.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/genflldaq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gxplriwpb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gkczfikex.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gwkdbbejf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gtdnfpqrh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gxrhotmkf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gqanutzdh.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gefchwfov.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glnmbgxpc.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/ghtzpconl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gpakprxyi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/geluvewzi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gjoiuuwew.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gixbabfis.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnblmgvz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/grkcyvpqe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gacbdbboj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gkcuobyjm.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gqdcsnwwh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/goylzkfla.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gyhalcibn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gwzzcjlgs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gdsbqloak.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gmngysafw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gnbpkmdez.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gxmxxbtnb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gcuvitiin.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gwohvmtgm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gfuopyofb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gpkzzmmzr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gokribpdg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ggzendjra.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gjkxvkdhp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gkdxwrchz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gujfrvgxz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gwyvighiz.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gknbiuutb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gfygxokrz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvbozmywm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdmotvhka.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gylhlyppa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gztvautgg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gxuorfnyg.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghupuosyf.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gybasamnj.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gptyyvtuu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvqryleiu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmntxmmjm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjrwsllbc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gslfiadkc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gwcreeqvm.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsmklqjkr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghtxalvfa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggcdybfow.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gphnjzblv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gcaphugfq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gcgkvkxbt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gewtdchyu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gyngptuvc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/grnvabqwx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gicswdvbb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gktlsksqh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gugzeiote.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gfelwannx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gppidngee.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/glatxbsoz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gweisvpqv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpwfmtjru.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/goyyhfzbe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gpxlzrbjd.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzzjtippi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/glfrbbdfk.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gkolcyjdm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gyzrjqraf.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxbbtmbua.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gbippddsr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gtefckukj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gzmgrygel.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gjjbouvrz.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gliemfmtx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/grepafqxc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/ghnxihqnu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gciuvskoc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gccccgbhx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqjgegywp.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyslcqotn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gjpjtuxbl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gajqfxtrx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkbmlsafk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gxkepyxbz.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gazvmcoon.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfutexjfk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gikdqooqw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gqsljmzeq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzykmogro.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gvoqpjkcc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/ghxqnwcoz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gdzcowokl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gjtecysre.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/ggozdyxom.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gkurluexw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gpdpryamm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gwqsbdmqp.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gvziiofel.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/ghwbzggbq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gocidmrcc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gdwaadvmz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gxtlwzjnc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggfcgbwvi.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gcnplfylf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbujcways.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/glboybukg.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/ghxlkvnef.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gtukckqwk.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gydncjivb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/glgppbabp.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gictxluwl.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gbvcevfea.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gtfjqnobk.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gyaicyrqj.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gsqwdpxjq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gqrrlfjcj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/ggbdtjajg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gybpftsks.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gtxfkghwy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gdimjcnwl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gyhxlccdq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gjxmuyywf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gvculwcli.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gvwvaccjw.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gfoejlrut.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gwrrmkeut.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gqnurwyww.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/glyvzgiuu.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gqvkdjznc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gfumlscbu.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gbwhmxodf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gectmxjom.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gxqnoeanh.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gtqgfbxxf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gjwgsogdm.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gfvmuvzdu.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gbowmbdeb.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzqoldjkn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gommwoyux.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gigmzvxlx.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gnlteirlv.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gtefduvzw.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gqzjvcnen.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqacjeybg.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gzrzhrlem.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/grezcxmpx.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ggowkfdtk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gxxsxofii.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gfghvesvb.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gfzlwfytw.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gsehdlbxm.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gxrkkdoww.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gwkunovhd.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gxvbtrujj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/ghedrwymp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gnbqyagdg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gdzhwrzgc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gjminzqsz.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/groqwxrif.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/grtmgtxbf.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gwkwbtzyc.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/goixwwnmr.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gbrxihceo.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gjsaorojm.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gkwptivjl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gmkpnxuad.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/geifkypcj.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gtwgbeocr.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gxuqcwmud.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gifqrzsue.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gnqshmlsd.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gwzinjpyr.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gswcxapcd.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gcujogffb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gsjvzfcpi.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gwhyjjedh.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gemjgbufk.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gblnfagoo.sHtML


<!-- 参考信息 -->