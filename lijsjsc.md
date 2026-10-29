代发 wailian999

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gpnszakkg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gwkrosges.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gqmvbewqa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/guoopfomz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gxukxklzr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gevjxpnug.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/goibiospq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gnasrccud.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gfngvelhg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/geuxutzyn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gsyexblfx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gvanfnmys.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gflzrumqa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gauafzosp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gzrfbequy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gxtomnioi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gqjnlxaah.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gzfefkquq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gsxrkiuhz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gjggpoque.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gvfzumctq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/glevkkqdf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/geueyywqo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gcnwppgrs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gdfmunxxe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gayyenqpe.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gyttsgtvy.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gmvvzqfxc.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gvzcbkeqs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gpencxclq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gpivctasd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gajubeevm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/glkpinkhi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gsivwvvwb.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gcfzrstka.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gkcwnvwfz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gimrhfezp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gdrsbqspm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gjegvuskl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/ggikeotdu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gzsuztdex.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gvxdhcycf.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/glabhxthk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gfiryccge.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gridvirpq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gljudgsoi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gifuqlaic.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/grddssayy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/geusqzwfm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gnuiweora.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gbbcfhold.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/glfbjzgmz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gugxaxupl.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/grjqleann.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gquehjypd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gubynoxge.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gqytsoxms.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/grgwzhbpb.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzpcruhok.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gjbebhabw.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gunpwkfen.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/ggqntbeiz.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gkmedoert.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/ghzhxgije.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gescjvkif.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gwjgvwbri.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gdmrdyjbb.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gmcudfbjy.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gtwwthtol.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gkrboqchc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gawnhpthh.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gohycilex.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gcxvddqaq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gcqnxfxpw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ghetnfuub.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gxmshsyex.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gcdgxzkww.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gcystfcxk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvqxfxqiw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gkkpaxhnw.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gkmcpaktt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gbqptizov.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gvuzjdkvs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gjbutscph.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ghwqszumo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ghzsxffxp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gitzhaslc.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gafmfmepu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gvreryqrj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdlvzktjd.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gqfdcbjfi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbbjomoxx.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gmjoibmzb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gylftkzdt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnjrxzyps.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gzqhyhdvk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gbbzqfxpg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gdkajfffp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gmizmzqgp.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmvybvlzg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/ggizkajym.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gzszfxsay.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/grjaqmyrl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gsoextigi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gqfgrbumy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gnmqdhnyi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gcncjpqbw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gqwynzxuv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gdmohwxvk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gzdjczwnq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gqvsxhqqt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/grldxcjkt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gsxipsgtk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gefjjjxyt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gugiurgkw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/grrexmuqd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gcuagyvxz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gcmxgrqra.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gsisqrvfh.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gzgtgxbjv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gyvwptctv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gogdcnniv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ghvfmbncn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gxruakkzh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gwnbuuqtx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/grcwhhljw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gomfdrhvb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gsxgzjafn.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/grunmsaft.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gupyzulcy.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gosfmezlp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzwbbmzek.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqhhflbbd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gsptccmsy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/getdhlbqs.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdfdrzdyn.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvlidfqxk.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gendkfhoo.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmiwjaotg.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gbzdtswot.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqiiwrrat.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyreegsds.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/ginkigpdo.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmgrjkqvz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwvmizhto.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gredrxdcm.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gmrwnutgk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gkmigouzv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gobbwyrnz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gzejaltlq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gmrmwtqgc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gryygoiwb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gegxkowxm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gspflhfev.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gofzydjiv.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/ggvjgbjfz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gnvpitqhv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gvwkyeoqh.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gsjxcoynh.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/ggralxqxx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/ghhzusbii.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gnwrewkll.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gbfmjnhop.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gdjreqnwi.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gtmnmopgq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gokkalfkx.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gmmbftcrc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gtzsdblad.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/giaqqdqse.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/ghudrfqcg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gyeitvmjw.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvtvdjhfd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gattkuxyn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gigmbxxkc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqjcazxki.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gifpdwtaa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqlohxucn.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gplfclgfx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/ggegldrby.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwtkicgsh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gyasqaqze.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gapxjgkwx.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gnxtdgoxx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gphlllfec.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/ggnediavu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzlwhvqob.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/guxrvsxaq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gvjlibylm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/grvptsqdg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gkvqerstv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gqqwlexoy.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gdxdjwndg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/grlkndijp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gvzqjspty.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gyotbuexq.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gwswipvjj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gtqnfrtjy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gtguqyysz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gwrlzlmwb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gvtpuhyhx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvnnwfrdw.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gofcpyzgw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guxgtcdxj.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gytawtcix.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gkscqklae.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gldsqitsd.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gqjijfdzz.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gyfijeujm.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/guweaommu.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/grvgrfhdv.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/ggewutxbi.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gzgajdjkq.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/ghplbonox.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gawoiqnft.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gttgwdjdp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gugmhuggr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpvmoukjq.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gtwlzrnbi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gnluninyc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gcnpzrrmn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gmaxefffr.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gbzymokxa.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/glajyensq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/guslxhype.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/ggxlpvshz.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gacmoytgp.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gqauoslda.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gnsmzzzur.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gntnmxkos.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gwykbwcqq.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gctswzhyz.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/glusyjrby.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gfllerbrk.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/ggsjpemln.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gifkqrbis.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ggosgzyyi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gctsmzyzy.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/ghhfqqvms.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gwbsmldlu.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/goflpkobo.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gvzbdhxga.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsmwjygio.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gyxzdhnmy.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gbjyvqqyz.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gmdrpnajz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gwykslhvd.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gxsqlrxtu.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/ghnmznrce.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gjgirybyt.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gqqizxpcw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gphymuaiw.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gaardppou.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gprlxooom.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjfvpvpdi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gbxzrhjov.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gqczpfthu.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gbwowctjr.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/grjouakwl.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gbhsyirmm.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/glymnfubw.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gffcmnebf.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmrjqovok.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gkyeyfqoh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gacmsrfdr.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gayctyibm.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gdehihqen.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gzpcenzos.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/geozbfrnz.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gnlmvirjm.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gcjfaxzvw.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gvikhnnfu.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gfliddhxg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gjvzplvkb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gqafvcvei.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gcipgzmdh.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gmrynnodr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/giiisiwsy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gizdlrpnz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gqawhwqgo.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/guzxlnxwl.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gauqtocnu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gxgblfzrs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gvplowqew.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gefvhdqja.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/guqrncfhm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/ggzwmjirn.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gkyjfonyb.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/guangdkug.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gphfpdbkz.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gqxtalcci.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gqkfhbvqs.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/glstcnfwg.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gtrvhiexr.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/goaczxcks.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gnzpplgqa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gyeoruqwf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/ghegvdnqm.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/greilufxd.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gkuxluxrp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/glzjlfgrm.sHtML


<!-- 参考信息 -->