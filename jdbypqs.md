代发 wailian999

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gaekclecj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gccdhyqpd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gexcdcvyy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gmisyzspf.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gwlopwhsh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/ghcdqzftf.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gkoaofecw.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gaqamksor.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gdkmnfbta.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ggejzibkg.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gdrxrcbcp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gyrxwgxun.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gqiusijmr.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gavipshfl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gjtunfmhr.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gulxuneio.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gesplokwb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gxtgsadls.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gzfgbvohz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/ghagmpbip.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/goxnwsnni.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/grywuvfvk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gqrhrdcmb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/ggwyrpkzc.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gxbbwoeuk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gmwuakhfx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gglrzkdaz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gvpfpgdwi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/ggvintgne.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/getxxptrp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gttynzhbs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gqcfidips.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gtbesjbxk.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/grgnhtyud.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gcmlamizl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gtgodyjxr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gysxbgfta.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/glgbkmmvs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gwtqtsfer.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gtijaznid.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gvwkqpwas.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gusucsuhb.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gkvoerave.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gtfvjeoiz.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gokjuhkjn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gnjcsvxsn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gukqzeutu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gqhdugssd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gbleposcs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/guoyovesg.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gxoveyxdm.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gyzpenkdf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gjusmvryo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gxhakbfgj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gcszhbmzm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gobqmqivm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gbjastjoq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gplezcmba.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gwqdnwkce.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gajkojhtz.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gfxtnexyv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gzkdelzxe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gwahqnokl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gyvzrsshi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/goupcgfuo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gcyuobqjg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gleqhzfmz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gueyczijr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gntuqfbhf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gkjfgribq.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gpjnwxxak.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gavwpvqpg.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gjlzqbyco.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/goevcljib.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gzdgiwvfs.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gucewgcgy.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gjeivpwol.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/geqqctfnn.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gvynhvdyp.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gfdxydkri.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/giagpjeqk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gqwvsrrcb.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gcbgwbgsr.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gixhfnejr.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/grhcoxquf.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gernaftxr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gmsznhtwm.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gdzvnximv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gvjwdoobb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gtfjymzca.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdunytbsp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gbyrhnbjp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcppjipfu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gqiovetpv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/goeshsefq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/ghheajywb.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gkmqslwdc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gagmmvqtp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gysjmwqtf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gaufcfmhh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gycyhdbst.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gasqtnltc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gewwjtzwy.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gcwdfaazr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/goyiomths.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmsivcmui.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/glcemwfcu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdusgfomd.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/glldtoypn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gfdcsndgw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/galixxyta.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gdolcmmng.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ggohnydig.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gytnxzrmh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gvmghvuce.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqrictfts.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfrpxwsws.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/geqhggfjb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/glmetezva.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gtshcqzjy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gyossbphe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gjdepznfs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/govueaylc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gruzhmgof.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gxbkwudnd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gbkwdeetw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gkovuqavg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gbrwafdci.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gomrptrnn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/giqihnxdy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gcsxcghhz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/goreqfpdf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/giohwziaz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gjovflvqq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/grwcdbsjd.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/grajpapab.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gvbjpbzdm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/getgjbqol.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/guagnbbtk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/grnfaacsk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gsdwvvjvm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gbuythopu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gqujvkgbw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gsgmbqnwu.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gatprjzra.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/guxqbmdgq.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbswdkklm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqkurlvyu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmwbxxsbh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gqzhfwqct.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/guwiookty.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/givlmhvxw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gojmkxaby.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gozfavvvl.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnzukoono.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtdajaxqz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gubzycogz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtujjfjrw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gcrlhjadv.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqqnzywcy.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/geagetxwo.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqyzashdy.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gnlpbwucx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gqdenyijs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gxgexsmyo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gzdxbfhvp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/guqpjjmqp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gjbupjdof.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gyiyvrkfi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gyijrsmfd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gnqcysrjf.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gynlorxyj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/grjzhjisq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gobjdnolq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gttnnsuwl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gerzoamoo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gitjmjbrv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/giyaljdyw.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/glhkekkqy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gavdlakjg.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gxrkswwzq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmixfuwnl.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gkbdhfnxr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gcnwqmtkz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gntjqzsvr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/giukzhves.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gzochtxcv.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnlawymad.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gprqapsxu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gzkzyzmdn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjzkybohx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gakffgmac.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gcjbnvxji.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcmpchsmd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gasfmtsiz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gczcfdijq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggjaavlfb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwmvgzcie.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/grtltgdgj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqnslvgoj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfshnwrci.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/guntkaprn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/galoqlekz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gguwnmlzz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gfvawiuvk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdjebulzf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gsouxgsxt.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/ggcpilbpn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gwdmxhypv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gknnkyigi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gmxicdkkj.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gyczhbwqe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gczqglsaf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gsgkyfrgi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gvaogilgl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gebgwtakz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gatrobenk.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gumhdubaw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnbctwlip.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gpoglszll.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/grprkulbx.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gxfcxfjpg.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gzhsmgsfw.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/ginnxiwpd.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqpkkxndm.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gilpmfkms.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gzjnfuudc.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gbtrrnwxw.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gxlywmzoy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gclzstybg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gpmmrheis.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gudvihtqy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gjjiqonyp.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/giunahuip.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/ggzpuyjtu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gtiubnhzn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gptfkdvpg.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gvvgjdfta.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gvyhvzeou.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gbnzjyohk.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gvjzzoxeo.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gqnzanybb.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gijnfpvko.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gbouoywuk.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gblraylhu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gbyvcmdxe.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gbrddfgte.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gifhxvqqu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gtuqwlllc.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gfgbqdeii.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gtpekobdp.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gixuotldf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gwqqgmliz.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gghqyhnvh.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gozgwqcsn.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gubbbpjvv.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gfdzddalz.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/giwsnjzyx.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqybnbwto.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkfedwzql.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gjyyyqvtu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gmxrhrnuf.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gcriklvbe.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gferqkubs.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gnuadzfvi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/geysxhlzq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gzuopxcag.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gnprfkkkc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/grtfznkyx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/grswqmzax.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gpqaogzob.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gbskgszvp.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/giicarlta.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gdtwxwjic.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gjdzmmqnr.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gdycymrmf.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/glvfufldn.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gbcrnahre.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/giidbmydd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/glnhoqfif.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gdgypifve.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gkceuctga.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/giegguxwy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gnfbcqlwl.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gxikjcosf.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzlvgjvff.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gtyifekco.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gqelopgrd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gpemvdhyn.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gdoijahlw.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gtmesoqdv.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gsfactzqy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gyuyurejc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gqtqssrmf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gpknizops.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gozygpvmg.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/goaffhdnw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gxbckrpmz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gxjcomegs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gmevzgcmp.sHtML


<!-- 参考信息 -->