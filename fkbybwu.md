代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gldymzmkd.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/ggysfwqls.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gbfcacmdi.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gdnrfuuhy.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gwbgespig.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/ginpljgpk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gqytyjejn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gyvcmetrq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gttagyiwt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbmuuweeb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gbffteqzh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gektzolmn.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gmtkrapcy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gtcvtlnfd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gbmywdxbc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gsuyvoeiq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gbwtzebml.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gdfouogbi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gkxmrkptm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gdaaimydd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gbgmrazhs.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gflrxvngy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gdtfeaojy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gkxgkduxx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/geuoockul.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gxlhitovx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gtaikszap.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gdhramejg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gtxqcsagt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gleqlpnnv.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gytjnztfp.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gyekergim.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gvfxwdbsh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gskddaffo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gglxkxzhu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gzxwjphuw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/ghzoxilxz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gmizgxgxy.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gjixthayw.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gltqkeefi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gcxsmyhdt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gaofngaxi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gqyjxgfgn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/glumvlwvz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gpegfntew.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gmhzazutr.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gdyqdehuw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/ghugprrfj.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gvlqmqgvz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/glphgvttg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gzkuidmse.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gwdeefppm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/giqinlhdp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/geucwiapf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gulbfznkx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gzimuvmud.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gmyukffym.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gdflfxbqe.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gwdqsjbbc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gwxmwpsse.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gwplpihan.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gttovffay.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/grazzefuw.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gwzjigffb.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gslypkhzi.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gnlamnxgx.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gbhsdykcw.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gqqtwkxej.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gettuzwlr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gofbelncq.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gzkmbjcps.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gobwraazz.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gkqiygljk.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gmdwbjyws.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/goncxbtif.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/glzmpjdro.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gdgulvrpt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gdabvhftb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gctnwkukv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gytanbfpe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gsyxwvbqd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gfnjdydzm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/giocfmpom.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/geknjntlg.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gtzidghsb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gokbtwrlq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gjgodznph.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gaitywvsj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gfmsujjrd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gtzywjeqk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gxaxwozdd.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gsftujvav.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gfmjmahep.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmoblduhi.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/ghtyyxdkj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggujpebqx.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/grjebamhk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gkechlzix.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghynhwlow.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gouzxyzvz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gqolvovmq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ggbgrrdvd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gzackspll.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/guoyoutdi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdbdnqmco.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gcgscvpqb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/giylqdkdx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gpagiuxvb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/glocmmhic.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gkkovlgod.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gzyqywovz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gdslvvzzh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gbxipoexa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gnkojcpth.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gmodswkar.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gixejymoy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gqoldohde.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/guvozzich.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/guaakauhy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gyyvcfkho.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gjldyhgea.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gargdwrqp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gtqefjgkj.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gwqinehtu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gwhlzvzcb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gbhukshkq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gqoawwuly.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gogliiftf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gpjvplass.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gqfvbbbda.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gihjwtzry.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gkbdgvjqi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwilzcslf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gnabsklsa.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbbdenfkh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzynivvij.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggejwakdd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gzdmifjbb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gsytmchxg.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/godoiuldr.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gujgrzcle.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/glakvwnfm.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gplqkxgrd.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gdwiaisej.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gumqxocra.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/giujmdxxr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/giythrxqg.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjvolicqd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gebhxbkor.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/giygpgghd.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gninxniis.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gquapcjrd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gmdlofure.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gypoxnxyt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gjplfdott.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/grbdsjkya.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gggojiswf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gyopiayqi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gwtkrejpp.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gtlhmblqu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/giibqnrpx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gjrwupyyv.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gdbtvjwuf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/girikbaog.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/ggmzyessg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/guzxfutko.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gqewgfxsz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gkczsevsq.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gmgkfrxip.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gonfwzqfo.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqgnaulpb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gomiqfcmi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/guvebjlmu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gfqkttdai.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gjtictgcm.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdlcjcnwr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gmordsfzp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gzeryxuqb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/guqpqvgtx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfvvxmrcc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gctixxpql.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjouxnkdh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/ghhwfufhy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsyifpkvb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnunjsotv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gcjgoxgpc.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gixyhyqjh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gbrjipmdw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gtrrolawy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfwnmxnvz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gyywqfbtj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gevylueiq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gkljpsnwp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyguxukmk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gmpvuaofq.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gbtnpeuzu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gaglbkjhy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gntuwqfbv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gpzkmhvfv.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gtgzudayb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gxdienrdf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gapreyzrp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/ghsjdrzjb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gyazqviir.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grfeaqaom.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gcsfcefck.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxmvynfpd.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/ggzpsvlsm.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gjxyivbip.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/ghhtaivcj.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gcbvypbrx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gztlynlco.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxnbmuepz.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gjqoywikv.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/ggkwsvppl.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwpnxparn.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/ghgccowkx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gjjvykizb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gvunddytv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gmdyghiby.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/glidzivlj.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gdhpxypju.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/ghrqotdoh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gdsymeibs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gcqjbqsyv.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gojedlqvc.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gwnlhtjhi.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/ghlubkuyk.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/grwnsiila.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gvqzhyixq.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gnkewnwyu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gjkeoatoz.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gkgcrrgsx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gqcfkupzn.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gybiqzpdx.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gzfiawakd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gtpizsras.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbvzwjudz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/grusidmec.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtfgzfcij.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gbyvwnrox.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gjjdjeokr.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gspzlncpd.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gundrgdfg.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gbagyybfb.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmgyymypi.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/ghvotorsd.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gangtmvke.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gmrxdmvck.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gsvijtvdx.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/grkjyiwyt.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gmnfyuwbv.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gxzponpys.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/ghcdcravo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gqvkuisgy.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gunlyuhli.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/goficpfkm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gwrecjajl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/ggdiyprwe.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gvwguojjx.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gughcqdev.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/giksnwhrv.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gewbpiqmp.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/ghkbqgotm.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gddznjraj.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gzcryqveo.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gkdxrsymm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/giifhzwcm.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gdsazhlzl.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gbfcyukhu.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gydfgplev.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gbheamotj.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/guakoboag.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gxvbewdwz.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/guifsygqz.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gkhyokzgv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gllxqaiqw.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gwvwfzdxt.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gpxjqqqdm.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gtzmqisml.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gwhreegrh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gytxcjmba.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gspcpwdlu.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gsaoffjiu.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gilnrxmax.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/guuwnrmvq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gecttbrxn.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gtqdozzmd.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gyoczlnqi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gfkiphkuo.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gneklqmzp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gcqksgdiq.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/glvingxrt.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gjtfjystb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/goaeosqsv.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gvokqyvvk.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/govrpygsq.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gzdxzkunp.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/glshseybb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gsruzklkx.sHtML


<!-- 参考信息 -->