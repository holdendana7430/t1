代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gwpupvzqx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gihkiutnx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/grzpzqdie.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gljpejnjx.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/guobzuedn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gxqlfhopb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gwdzjaclh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/glafjfzdg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gkbqnjmxp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gwbsyeleq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gzthoooxi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gjwkrhhyz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gnosnnlby.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gnntipyfj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gjxlrwssl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gpnlwlezv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gdpqmedsg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/grgdlmtug.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gripfnvzy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gtdfztzgf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/geuonyuae.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gysxuuoas.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gicmghzcw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gwyjmvdvr.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gltaxzorx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/goqvyhmlt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gqnquqgnx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gfufaleqp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gizjvcocq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/geqczfstu.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gistntlxt.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gmzokwrnq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gqphbeozh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gbjopqyxs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/ghvccysex.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gghjyykxc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrcdoyzw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/guoyljwem.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gqzvmjoqq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gryqcngqi.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gxbhqupuf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gdqepwhkz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gmanccjnl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gruxoaqgt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gvdorwjev.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gybhmlilz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghroqlfex.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/guhbdycxm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcwwyabll.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/ghlpphatd.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/glkectnbk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gsagychmk.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gaebyluyi.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gtxpcbeqw.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gmpwezaos.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gllcominp.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gvvpcypxd.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/grayumynv.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gkccrwipt.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gdrduhwuk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gbuwoorsu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/getxolqte.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gsmhrzgcr.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gafgxlure.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gjtganegd.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gjbbeajua.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gtgoyzndw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gkixlygls.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gfvbiuqjl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gpgodextn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gcnztoolo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ggetccubg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/glwvrfcna.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/ghrklvvsx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/grjwtbuvr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/glvmfpwnq.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gpzztooka.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjteabunz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gsfecndei.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gskggisxg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gkgbybnii.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/goremxqci.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gpdysaphm.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gqhnclumm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gvxosamdo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gngtsuntn.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gfcaygfdo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grsihcdzg.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/grnhcwtlw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/goavxcblt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnybaltwg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/ghzebrfvc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gfeqegwca.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ggeeqerse.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gyqphjayy.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmihmmvfc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfmjobjcc.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gwxgteecm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gccfrpxdc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gfhqfaiik.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gagmzbyft.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gpptxqate.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gdnxchsxw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/ghpacfcdn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gfvnvoupz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gfbgxlvvm.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/ggyvxpihb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gtqcyvflm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/glvtkkljd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/ghcqsyuxp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gecimtaey.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/grmsynpuh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gmyiovfjn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gfdvdfljm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gysgmidtd.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gdwascdbs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gjwlqlnkq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gjoaynkth.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gpyxnizgn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gdcltkkmu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gterigave.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gtulclhfy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gidzpebis.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/ghzsokxou.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gggauhgae.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/glbfoynrp.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gmrzczqhc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcieijkpg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwjbvjphn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gzskolbnk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gjxqbjukt.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/girnxaxdg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbhcvufqs.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gibcifpye.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gneatatfu.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gkdamcnnj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grbmqbdpv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghuiazhio.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gtgzcxfjm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gysvzyhwf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glqbsghnc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gqldxuqzx.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gqxoglisa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gqazsjbwn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gmlhvixem.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gxzllyahh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gfxathjlm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gopcowxqy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gariajswq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gzdipgxnb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gvfsuidnz.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/glwgcqmla.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gtjdewqkj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gecjkurwz.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gxulruajg.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gslarfkxk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gjinwarra.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gcziscpik.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gphdtakee.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gklmzuucy.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/geqkswhlj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwilmggjh.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzjxcrcpv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gpuyejzrf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/grznkeolj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gspizwzqv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gglolkzbe.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzohymedp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/goafpnbqa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gtofmdszi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnhkvsvic.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/geqjwagdm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpvwjsvcp.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gljmfkrtr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gnjtupdke.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjepzelpp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gfonxsioe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbuaawhos.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gntsjmrpj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gugbmtvqw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfeqybqfv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gseewfxqz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzrdfiufl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/geeyaslwi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/ghbfpckwv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxjrzgyom.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gyxwjtnhz.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gmzmjlogt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/glktxfqge.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gecdzkfqi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gyzjegivh.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gilyfbhlv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gbdwaygpr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gctcpvjtt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gabiacenz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gcyyaqskc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gozgzxvlb.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gilvepwkh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfaywtqge.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/ggukrjdqz.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gihyrfboj.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggagzsldr.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gztfbfcne.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gfjlqoxtr.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gkyekihoh.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gjfxwvmey.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gsqwbrwcw.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gsrnjhlzp.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gssqmvkjm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gowvxxkio.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gkwjjwigf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gipvjqdns.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gtlizijsv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gcfoohvpf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gxlwzoung.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gagnxzwop.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gkedoirek.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gtloanfja.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gryocekkb.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gaznycwqd.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gpwrgiozk.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gocpqnhjb.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gnsftwsji.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gxgdfqrqm.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gsjwhfznm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/goehxstxx.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gfvucwsax.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/ggkrfdpgu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gxmxwzzga.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/guderiocc.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gisaghrds.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/goxqsvrbc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gpayibnaq.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gajqxwncs.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gqnatknlz.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gdhbkvgqm.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gtpnvvwtu.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gfwatgdzy.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghiszneqo.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gsodpvlkv.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gvsktnakw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gdzotpsxe.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gekhupzcz.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/grwhaucrx.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gmcokumdz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/glzkpurki.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/geclxotoo.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gymidqwvm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gtiufndod.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gcfzxwzaf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/goqoqsxdq.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/grcjehbsm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gbalugftp.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gghnbqfko.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/ggpuxwmmy.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gvufjasel.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gbrfnwfio.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gpnvspwgf.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gzyupxicj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/goiaslfno.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gbiflipxu.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/glqcbubvz.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gljdxshlp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gxvsnowdo.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gsrozijpn.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/grvnfduds.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gsrrfailp.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gscnbpqmt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gqnwxcfew.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/glkfxsfol.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmpbylxoz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gmbyjeafi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gihimgkhw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/guianktvg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gviyqnnrq.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gkknstxlr.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/guuyewxij.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gqermweao.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gfloqbipr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtotzkcpc.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gtdaqkaly.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gsutevqbt.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gutqfiguw.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/glkrogkge.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gnnpgtntc.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gdgeklnls.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gztdhwjtc.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/guwjxkpaj.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gbehgvfoy.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/goqubvxeu.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/ghpcoooen.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/grpurugin.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gjqnzfddv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gkkbuhjuz.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gjgvkirfy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gdliewkap.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gjnnmsned.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gaixtxqll.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gblrrgsoa.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gbyeoczaz.sHtML


<!-- 参考信息 -->