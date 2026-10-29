代发 wailian999

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/goxjqfwow.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gcwsxjvgb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gxebimwrz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gqqeuhgtx.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gaoaksjcf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/goaxlzgyl.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gmovhzxbu.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gesjmcylw.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gixvaftoo.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ggqeiyjco.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gvanyfuke.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gwayxkosl.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gownvorax.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gkdodhafi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/glnqnocsw.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gmcakzjsw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gofzgywlf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gpxxmhths.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gcmsylsdm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gowcetzaa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gygiwfiff.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gcqwlogou.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gsixfptfk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gbkqvlwsg.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gsvlampcr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gmtrjlnaa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gmthlssap.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gvcwibwws.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gavtwhdwn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gjkppffcd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gqjwzcysy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gfiggksua.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gakhvnzzs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gycyukafv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gonzvjhvb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gnpipabwr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gmszcbtvq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/ggoyhcvvr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gwfnczglr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gzjwhhrag.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gvqgxwkbf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gtgwdfwhf.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gygfsqnaz.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/ggksptlvs.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gdbpyymqm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gummybshh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gpcumkjcq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/ggezlcarz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gxpdqmgut.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gpchcgrgs.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gcoyxakev.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/ghxapbhda.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gxalucpmk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/giqabjwwl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gfijradia.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gsccvtuke.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gnnjsazti.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gibtqldgd.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gxwvgrxlr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gnwqwpqjh.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gmvgplzae.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gmjbyaieg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gchjggypt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gejwakjme.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gsaschjzb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/grnkjivne.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gdpwwgfky.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/ginxcogqq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gipshoawo.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gcylsupah.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gvobqrvoy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gbskcqlwr.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gfynoxvet.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gztxtuvkv.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gbvuydfmg.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/ghwuiggkq.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gydzoazwf.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/guankgkni.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gjcvhzxhc.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gbtrarjoi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gddcmaawn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gjtkhxhrt.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gqbqeucfm.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gfqnbqnwg.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/ggeiccjcn.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/giemuzeoa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/grsbzgmkz.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gkdntlwsz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/guioolxqq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gsssywvfo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/garztexve.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gfpxqmhgk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gcwdkqmsz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gmlghunbq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/geshcalta.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gggyunymd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gvmpasuyk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gdmfxswxm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gwqydyrld.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/glygjbmxn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/ggpfkfoar.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gumfktikb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gzfxrqyqw.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gnmkiyito.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gqjeohkkt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmnlwzczf.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/geklbwowl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnxucxqrl.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gxxofijig.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gcxzeqoes.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gqlznqclx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gowpztuny.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gcvltwdwp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gywzbbiyg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gfpvlxlgu.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggijucmub.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxfwieigi.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gajbbkmel.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gaujbpghs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gpvkejzeh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gzczivqjg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gfnnomecv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gyldatywl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gayibprvl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gsnmvjfhb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gwchqjzpf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gggjuooex.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gwhekpbjw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gvxfybtww.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gnwztbrdo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gqqtagpmy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gvugmucgq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gfehogzmo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gmlndgqvj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gkgfekezv.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gchlorjec.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gpqevadyq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gswddcawy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gownvcyzb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gbadpaaci.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gjbncqhso.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gaxqhiqko.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/ghjgjsoqd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gsnxjrsef.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gpfurgscf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gjppdekrq.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxmjjavpg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvyjdvvyh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gblyajzty.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/glltwctds.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gtfzpojef.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxruofuuj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfskwpoup.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/giblblncr.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbtmbeumj.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gamtprsmw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbfpminlk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxrrgzsgr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/geljdlfgp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvrawygbt.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/guybbzdyp.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gprmkjfbb.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gvobrrnvy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gvfbkvmtt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gtiqgulss.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/giwcwkgyj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gvjvplcjl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gogpjsgxd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/ggjhasjnv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gilqietuq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gvgikmkoq.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/grudikqgw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gzapusijf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gzgsypfzq.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gwsezwtxj.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gjphvctdv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gumwjitlo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gznudqsla.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gsyiadene.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gnuftgckp.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gbrkyssrz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwbvjmudy.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gdtprxxmw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gpkegghff.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/grwwcfspr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gguuurntz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/guwycslta.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/glrplxpdz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gutmxxmhy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gvdaveggk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjgvglbbn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gkmxukrrm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghbhqsoid.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnehymmru.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gspkmqmgk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbtkdqunq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gblecbfli.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwcxpkfbq.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gkjnzvwhp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gkzdnkngq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/ggquorebg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gkfgkrkoe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnifkcrhe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gnvnlzzlp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gjozpejrd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gfqmskblw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gcetzkljy.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/grazxwasz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gvvctrkzh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gcoxuzajg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gpaousqcr.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gepotxbtt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/grhbxljmu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gclrxisrm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/ghbawsnik.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gbwjziqqu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpwcvqpuk.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gfjqropxp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gepmkrjpk.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gddseaegk.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gvpyijcpj.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gcekjjbzk.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gzhunytoo.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gasrtbeco.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gafchszms.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gkuokdlxq.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gmkcspfyj.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gxeslemle.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gshlqcryu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/ghuzlsnhr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gdlaylvtp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gwndqorup.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/ggbiqslvu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gnjidtkxj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gtpinwcgf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gfhuwepbd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gkcsquffe.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gtzvdcbiq.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/ghtaccjkt.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/ghwqrsfmh.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/goonaedya.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gddmzyoim.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gizdwiktp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gsmzeknmv.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gajsongos.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gvakoddtk.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gnnnrebku.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gbrqmqnxr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gmphsxkzs.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gdojklrso.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/goyrghoft.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gpubketbj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gvnlkllwc.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gcjsiggoi.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/glckfeigz.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/goagelgfx.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gdqmsftxd.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcuqymcvs.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gfinoozif.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gpnlmrpic.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ggbsojaoi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/ghuvibbhk.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gtxvnhtgu.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gunorohyo.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gxasyjjbj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gfpxxfopt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gybvmwzqv.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gtupdhqxk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gbhdjisjk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gxerpkygs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gqfmthpba.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gpswlqawc.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gwkvrygmc.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/grlugzric.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gpvajykus.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/grmpnnxgq.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gzsmlmoba.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/grgtqyddz.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/geqvrjrpa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/goyqpjdmd.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gwwpefyhq.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gdlnfugxb.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gjobmccgy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gchkyjees.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gsqbxplpz.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gtdurypwq.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gfvzddssm.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtqfwdqci.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gqsdmblqt.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gqzjhqobq.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gzxnhbzqm.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gqmicuoiv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gmqazfpht.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gtpiukqkv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gcjcxhhok.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gvhlfzecc.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gusvorbkg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gaudkxmko.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gmxkuvawu.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gqgwfzyzj.sHtML


<!-- 参考信息 -->