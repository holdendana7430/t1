代发 wailian999

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gfvpefxff.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gldhkfzyi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gwobfeala.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gnpknnocn.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gwwiurocr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gfqglcszm.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gsosmdwcw.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gjpmforsy.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gbksrzdgo.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gqbfhzyet.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gutkntxvb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gzamxzrjd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gkatkmokv.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gbdzyzhpc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gcaduxzji.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/guzpaneaa.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gcmiqlkkr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpbtzxtic.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gmgxpnrci.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gopyzrzab.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gxdlwllcz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/galjnaubx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/glcicofak.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gssxucfzg.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gbmxcgnzb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/grnnomqns.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gtpkvwmpp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gqppfqfgz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfclpeyec.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gbvbmtckg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/ghpgnpscw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gxufxwxkg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gfcgeebor.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gqnrmrvli.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gmpxkgwxe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gihqkeeai.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/glhzokzej.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gcuyhgksh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/ggdnxlgui.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gthicdpcl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gfvzveomt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/giacnjglc.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gijvxbleu.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gvsgslydh.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/grnhwsali.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gpemgmjch.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gyrwxbfdl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gfifdbrpq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/glgfprxnn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gxtyptnni.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/guofubtxg.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gluiqetmr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gewewmjbh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/ghedpamtd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gtbhhynpc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gsnxjmqjn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvyutftce.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gcuhyinmf.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gokqelhjo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gshpivttr.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gjhirtspl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/grkudngey.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gyvlefewe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gcwotdgqu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gdrpmowhd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gpfwpxosw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gnvbedkyw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gvidrlxco.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/grbdtibbm.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gjpykhosk.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gwnkocejn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gyztbpqnv.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/govntmmmb.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gkcjogeyu.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gnvunocuy.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gzxuotkmd.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gagxjtgez.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gpamqmlxy.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gqmvqonee.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gdduakjen.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gxcrezvxj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gwdumgwel.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gqrewhods.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/guaegwwtc.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/glzhqimzy.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gwljstfsn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gfxfajdwg.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/ggeddnutt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gxnsidpyk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ggxxoqnuf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gdvecslbj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gtdhzrccb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gabkvsjzq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gxoiwiblp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/glnguxbop.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gglvpkjui.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gmatoxhnb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gspehkzzg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/geewlcnag.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gywyikvxv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gctlzknvp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gwkodhdax.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gtxqhwwjo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gnwmhwygk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gajzdenqv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcwxafcsw.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gglhgrcdm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grjycyllp.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gqxqeagum.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/guzlukigc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvusaxdkl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gchvqagma.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gdbsqiemk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gdyyvhzzs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/grmqhzzir.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grnpzolzl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gpwblfscv.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gtczjrsuh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gnamwkftd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gzrbtyqhx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gifkpzkro.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gdrhfazzs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gkexgmzue.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/grhihdqop.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gmkxikcck.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/grkmqzrqt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gixtsoubl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gjdqgocav.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gnajutzei.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gqppzjctc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ggezuaasb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gbdlvybwx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gdaceubjl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gyagnhrll.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gigwihxnn.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gmlqkwbbc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gotiwhpig.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/golfeyczj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/grbjfkhlv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gzwyfmgwi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/godapiast.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gqpgagdwl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gsfoyrcnc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gccqrrhms.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gqysfpmgk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gvoegxhwb.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjxbpgufi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqefanbyr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glapwacti.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gwjllzhys.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gppebcrjd.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghvoqsiol.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxpwznokh.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/ghfgajzif.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghuzgsfoy.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxvlmlbwz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggeqftopx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gonmharxx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gukeefiis.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqbqacego.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtigbpsbh.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtvrdjzkc.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gfpnxdvwf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gqabnrvrf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gtwtgdkfy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gehbejbjs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gpzjicgxx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/ggocegwjr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/griyyspzw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gfkknclba.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gqvtszluf.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gjkrejsye.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gguazynrh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gdhlmwarx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gescqzxoe.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gjahiuijq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gasifnygj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gmgmjaubc.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtqfxatpo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gsnsxmoge.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/ggvgmeevg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwizmfsph.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gkblvhodg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gweqoandg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/glmwpcawl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gtaqgolqy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gjkbvcxqy.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbhvcdbkd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gdcwcznze.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gorpdfsmo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/glucqyupf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnjdxeljj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbpbvvmsa.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsmeatqkr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/ghwhlmtpq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gzhaeyzor.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcjzalfrw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxaftxyrb.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gpuvdkqhf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gqykmawxj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/grpxxkjwe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gpkjaaqlj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ggncozjlg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/glzfupzsl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/ghhwuutqo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gavuwrhhe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gkjrcexrg.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gqtaqedzp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gwmucgvgf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/guuvcrlnf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gyooojcyc.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gpmkbgbxd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/ghtdpsxzq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gimjzqzjy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/guworrfdm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/guuexcgwq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gidjuszbt.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/glvevpyud.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gonyptfpj.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/geakmxqqg.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gliwyjbjs.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/geweithfa.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gmktzxfue.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gbmyfchdv.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gxnqycstr.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gibizplvb.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gsllvqqtx.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gjuhvpbws.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gbijurmnp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gjgmpxfao.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghqxfbotj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gtxpptjnf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gijpttfjx.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/guihdbikt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gapwltapc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/grfczuunr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gscutsnhf.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gmuelqwsk.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gltqxfdfz.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gxfokvspf.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gpqirixfx.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gcoeuqloe.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gvbxgfiwj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gpturywcq.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gtkhfbugg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gjkjlanph.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gfvqhicyz.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/grfbivakj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gywlolphr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gtzurzdlr.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gwptccyiz.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gsejcuxgm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/ghyizibkk.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/guyjocnok.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gnsiimycm.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/geyljfwgb.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gttqwfjzf.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ghyvktkgg.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gyezxfzed.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gscayjfcr.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gnpeukcrl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gwarpgpax.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gsehlpvwx.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gtqtxytjl.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gwkjqzyrt.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gonbzguae.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gsjmvtyok.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gtguloeep.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gehwjfmmz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gvikreevu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gduckiomj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gpbwwcbci.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gewbdkysx.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/glijxfrnn.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/ghgjmcxsh.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gymxedfyy.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gwqupyquc.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxtnbgysr.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gulzxaljl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/ggceuwbly.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gwouephbe.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gtjyvwnhy.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/guzqaijai.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gsqwkutcn.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gtrqvcwwp.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gorfoznuh.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gttglgdic.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/ghfixtmkw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gjowdnfag.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gvjucdrsb.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gyxdoqgtr.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gnzmwzvdm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gykkbeofd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gmomglsga.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/ghrvdumwx.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/ggdcnatpy.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gebkwcspv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbdimlkgz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gkxfvxeef.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gagxtbkrh.sHtML


<!-- 参考信息 -->