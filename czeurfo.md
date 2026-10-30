代发 wailian999

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/ggnzdpohb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gssblldbv.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gsnadubgx.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gcvrqtmwa.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gfmjcroru.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gqttqhttf.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/ggbyxttiy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gvlfnfjxj.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gdnvhwpcv.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gdkzlhjdq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gsawmyczr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gnhpmowcu.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gzzjuyqnk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/getulswid.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/guywnpqag.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gqbekksky.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gkokyfqww.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjeovrtrd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/ggatnhpml.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gmptnutjd.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gmzscmduc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gxtcrazxs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gaokrbrka.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gwhbiaqlm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gabnlrsoi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gyzjfqvfu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gclowvkdd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gpjwhimkm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gjbfqlizq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gibfzrqvs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gkccwtgzl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gcnaaguld.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqsbmjd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gwcugrwop.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gtrglumgy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gteqcwama.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/grjwljgem.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/grwzchiaw.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gqqtvpnqn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/goblxpqkh.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/glauyisff.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gdbvwrccc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gyrcjntgh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gpqenncip.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gociognoo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/geqgqwpzr.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gqvhxdegx.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gdmxiqiin.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gbzlihlmg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gsgcneyvq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gtdlventr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsvmjxcwp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfjsdswkf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gonhfdxkq.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gosvvytgd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gzfcbicmy.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gkejwcrkl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gdniscbes.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gobtkfzhk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ggbgafwlf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gbulanmac.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gobtdbufv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrnoozpz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gjtnqdsqx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/giqczhbhg.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gitrqtjkp.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gdpjmcxvc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gbywyunkc.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gupwzultu.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gzltftvve.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/garlzwpfj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gljdsnqvw.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gxpoaeiyd.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gbfliwqas.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gmxxfnhaf.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/grkvspmpn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gjldkfmzb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gsfdgogdt.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gkviuaclm.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/getmqyanj.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gdnvxciox.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gsihigbih.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gdyucgwff.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gotmnujmm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gbgippmha.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/goyvsfjzs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gxqpaayyf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqqqpgmmi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gjfqkuhnc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gsckhvgbq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gnoicacdf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gnixapuwm.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/guufruapx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gmynhtstq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/glwdbslzb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gdakfambh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/grqchnwvk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/guprujgfi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/ggjvjuzfh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gzyqitjjw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gdsqoftpe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goaejtrda.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gmwxfzplv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gixawyjqb.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gjgkkhusx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gxamwiflj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqknemjfl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gdlkfqqgg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjtqwbmyh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ghgbrbost.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gwitnkylu.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnfxvxluj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnwzbdneg.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gkwbdsjmg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/giqwnslxu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gdxytcalb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gljdwldig.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gkszjfilv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/glsorldjl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gckwvyldm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/glghcublm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gwmzchnuu.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gquanxhpc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gszddotix.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gntjzbwbz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/girfxlece.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gyyrorueb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gbsmkpwss.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/glnfdwoba.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gzxfpcwaz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gdpbqgpjw.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gcrjcucah.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/ggnokznuq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gqpfwazlv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gsmyvbnqp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gloektxan.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/giugrjrpe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gacxelkzq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gncpyezwv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gjyugsyoy.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/ggokvacjb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gkvtvwzjk.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghdlquthp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjyenukrf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcalfreff.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/glzhrlemr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gitvmfiwp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfvoszevf.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gixiswavw.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gtvuizfec.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdixnaweb.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/griqfpzzx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gowdbitbi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/goxrwtbjw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmvnfnmiz.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gybetswsk.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbbtkxzgf.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcdpewtbn.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gioakrqzy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsfpilcg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gnzqozhlh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gupmuzbyy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gcmnwmefo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gcnuvcdbv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gczxixqxi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/glushawsj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gfgkcdcxi.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gxttvutre.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/geysugomk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gdoxibawi.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/goldzwwtv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gnvqbgzox.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gdtztxizn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gzacysqxd.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gddevogwr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gkcsgffuv.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gldwnvpqc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxqoamxzw.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghjabowkt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gkjzwxqbl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gqjljuknc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gahameoqe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/ggnfbjbes.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gssvupfhh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gcomexnks.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gprvwehlq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gldrbjzbo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxauwgeey.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gagcbixcu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqrlmaorg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/guntgvjeg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyflxxwbn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmkhyumyg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gkxjmazpx.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gshateaqx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gytzptgns.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gsorinygh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gsplyrusj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gyuqvmsrv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gbmgnbcok.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/ghodewypt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/glllaliso.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/giammvpyf.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gpkckyihi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gmbjibgqn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gkekhdboi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/ggvvmnjev.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gwsyzsfld.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gyfifygjw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/giogobqjo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gbowzcccz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gbfsaljqt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gefphazrb.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gbwzqdlfs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggoqhvhaf.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/grjihplbf.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gcrepcwgw.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gjhgbdqgp.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/giargetce.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gkxwxmoxn.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/giiznbous.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gfotcivaz.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gciojoaay.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gehynvohj.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gimybhfva.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/giuegimqw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gqfwaarmj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gourrkbfw.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gkvjtqdtq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkytudpjx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gevbbqqjt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gpyypsqsd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghaatruzb.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/grhymsmne.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gnimidmdu.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gnxoyqzwb.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gkujmckla.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/goypcetws.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gvexqjueb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gqmjcfflm.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gumnkreve.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gttneqagp.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gejrbtlgt.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gduihueoh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/glidjhcrj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gjwwskcto.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gbmnhtdef.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gjuggkswi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gwlojzubr.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/glcyyeqoy.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gznyckahj.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gjbbhrweb.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gsziofkde.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkmxpjjiv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/ggfjwibqp.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gydetohyb.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gbtrezube.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/ggcijrilh.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gyftwexqw.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gyxhcbpdp.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gfklbmphc.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/glhqmnmjv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gywnwchst.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gwibtrhdx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmiskvfgt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/geclvmxvx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gzltplsbe.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gxflfmgqx.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/glwxxtmus.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gabhiutkb.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/glvfvzryu.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gumyyphra.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gwlcmhbtz.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/ggkaxnojf.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gbbvroapb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gzrejzzsv.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gwaxnxgjo.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gvjpuuhkl.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/grbqanfac.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gfdxsptmw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/godhnszej.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gtrevszok.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gumnncnrh.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gtczxblas.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/ggqjgoxhw.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gcbopsazf.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gfgvbbsuf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gaajhlgoy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gbkmyxruk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gskrapfib.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gqxsdaicg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gthhojnzx.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gxzaphkti.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gklvqnppe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gwfxykhic.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gdcgewxkt.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gcrhmdgcs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/guclwnrcv.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gifrcbvjn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gulwtbdbm.sHtML


<!-- 参考信息 -->