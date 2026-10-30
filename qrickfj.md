代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gpuqcwrur.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gowrqxdox.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gupczdymg.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/ggfsxemfs.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gfouokccf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/grdugqsid.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gjgxqxpgu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gybirrrcx.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gnlmysrfh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gmtiprbmx.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gllqibavj.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gdjcqpvuu.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gnvhpfqqx.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gekvbtyiq.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gngnemxik.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gylxmpcwg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/ghzzmcgro.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gwyjlrijd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gtreokhoy.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/ggaqryjvz.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gvbyxhvfi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/grcosqokz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gizslacgw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/goljvodev.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gbxegqrbo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gocqaknat.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gewitonxm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gnipgvkqz.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/ggeuklqsp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gxhicwhab.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gqdrlqtut.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gyytgsuwr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gqwankhml.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvedfbqs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gqcidztep.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gfvsisips.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkqbvjgw.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gbyhlfrgm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gxckwwgju.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gokgyupmo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/guecdidsa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gvutwwawo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gyygbratz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gdbhlnkhk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/glrklwqon.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gfvcusaoo.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gbtociavy.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gvaxszytp.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gqyaeynjp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gymlfokxx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gckxaudlm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gteqmwowc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/ghqlnwmkr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gyzfbgfbe.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gozoxdafr.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gaslnnncy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gaiibocyw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/galzuvyau.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gkjccdcyu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gtsssaphd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gjhrkarah.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gwrpcjpfd.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gzntfvgtl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gyoicsakj.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gttzdsnto.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gjzmtfkrx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gmfkytuhn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gpsxkpmxa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gdhhwcbgd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gjusxvxbg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gjrxqwysp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/ghwnpozcb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/grngowgbo.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gapaquloj.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gqkevemmm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gajxvgilh.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gaeoaemnz.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gujvxdgwl.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gznapunpf.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gcrsnprev.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gneyjawpm.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gdhtelzdu.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gylxdrjqs.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gobiflpqz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/ghcxqyioj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gbkshgane.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/grbwjloee.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gpyhgabhl.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gvpvlcomr.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gmykyshih.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvxjkvgaa.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gcrqnrzoq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/geesuityl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gmipfhhvm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gfeuqyfuh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtynttbtd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gzsplgpgu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gorougxqi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/goywyprca.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gxrtyjics.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gmdstgglm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gvsdskefw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gadoadgrl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gtjadltye.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gykejiiap.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gvmoiofdz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gljbbqhwn.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gtdcqnupd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gxygcgmgz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gydcesael.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gzjxvuvgp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdxqiqdba.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gobxabopo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gwbfrxmjq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggsomfypk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gufgemelg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gjodknnwd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gqwtofqgy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/ggtyfnfrj.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guxclkcyu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcsmacmyl.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/ggcvvpwhm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gsepatcuc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gtrcacezg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gljvhmjim.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gzestldnf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gvlcdjvzi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gwxhyletq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gjtdbazyp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gglsdrqcu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gkeyixpgf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/ghlzjqube.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/glstbkynk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gbjzluzft.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gqxsjinga.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gtfqlpume.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gwqoemxyy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gitxbfhxp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/ggnvqmzrv.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gezekmusi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/glgqoanxy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gvdiudvxf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gzozlgaku.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gaijtlknq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gfqkxtvqp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/glkefwyqh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gqlwgbreb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gfxlpqejj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gzkmrzsub.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gqaqghfhs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gttjqgmxj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmpdvszfh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvyacoxur.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gasgbcbzr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gmsaxaeoc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqubkwacw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdtayepff.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gvhvnsnxz.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtnxqiiak.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvwcleekr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggigvqvoc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gloediaab.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/grxmoqoar.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcbxfebei.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqafeuiir.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/guikirpgg.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gqgoolgti.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gilonyato.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gidhxctkl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gkcskohyj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gcimuowul.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gqnwkoctp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/ghmvjrulg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gsrjhcezp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gjlentseg.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/ggmfaxapx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gcipzbbvh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gyyjyttgw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gylleqtkb.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gyrjbegvg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gjkqpqckx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/ggrvmvqih.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gvdlrcqme.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gvdfxwkcq.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gxkwkzwvn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwrrsmvdc.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghiywzblb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gzraqcfuz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gzfzocyhd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gzdqyxncn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gstsdydap.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gozhfqduk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gkpvsrmhm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gavpzkexv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gazofswxm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gniqqkzme.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzceklzyi.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtnbjvjum.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gvxlodktp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpnxxlirk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmzmgtinc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwnebuqls.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gwjejqpma.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ghscvasnu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfsbcurip.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gvoegrmez.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzuexaoak.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gdbcqrsdw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/grsofngvw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaofdehsh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/goccbccjt.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gffgckhby.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gimntybqc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gpkqqjiqu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gjolqpfxq.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gumpoprvx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gmnfwibvr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/glvkhqofs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gfbwlbrfs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/geytsatvw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggtochkkk.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gsqtlplok.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtwijvwrt.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gywfligpv.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gskrmpbqj.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzeyhqdwr.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/guprjwnzb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gfuwesoif.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/grgtosoxr.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gvxafldjt.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gpytbkefs.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/giocthbsa.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/grexaiigi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/ghafxcxlf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gqeixrgqr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gvlxhtbcp.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gbxsybgse.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gtlostzvb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gmngmtuwf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gxzwcrzww.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gkadpxvvt.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gdknhakin.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gjododldz.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gxayuhcju.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gfwbdfxmt.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/grqmaiyyj.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gtqqzypgp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gzqgsusxd.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gdkdngvkk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/ggydnnubg.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gakymtrbr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gllnlfiln.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnbgkozik.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gggqukamg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gswlwripy.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjorbozlc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gaouhrysy.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/giaxqneng.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/grkarykjx.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gfslzzkuk.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/glwiglaee.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gtsidkfpi.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gonbelylq.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gpddrsxzy.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gunqqvuvq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gxonujqki.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gqttiptjy.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gfhmostpa.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gsurhnoli.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gqqbvbxor.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gyjebwhmv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ghclezlmz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/glbiwcyie.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gsuxjnmko.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/glyeotrxg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gduwyktvl.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gyvwjmrsb.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/ghttlhdvi.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gdfzljdqm.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gpuxnupkt.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gokaqkkml.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gjwbyxinj.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gsuavztfr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gqfwjxdjr.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gwawubybt.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/guqtgkvfj.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gfgmwgxpk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gklthuljb.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gbkssgzef.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gzdbpkvnk.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/glovrhxug.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gnrqchliu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gjqgqhsyx.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gywizmdbr.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/guhsdiukf.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gaifsrxtg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gktrcavtr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gpjolxjla.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gcqixybed.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gmkfbpvfn.sHtML


<!-- 参考信息 -->