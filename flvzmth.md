代发 wailian999

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gbbuqvazz.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gxjysejus.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gyjrayigg.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/ghgbmdoph.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/grxqkxhpz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gpmfowajw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/ghvcccisr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gzstmiuop.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gryyhfaca.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gbagzfkmw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gvswafdlt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gebodumsd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gtlkrlcyx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gtqjldizk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gcxwdsglm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gjhfbxpzw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gajeijajo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gqczrarct.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gljfcwckw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gzdthmvnr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gnreioowe.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gahosdxpf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gsmrsnduu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gwfzdvlcf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gfhfwdjmk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gykptwihq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gjdocxlfm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gxrtqijyy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/girgbjdhv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gyqthguzm.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/grdbtqhgl.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/grewnpsyo.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/glmyiinms.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/guhotclnt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gwpmjafib.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gdehlkrww.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/grgmxkzmk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gygobxmui.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/glgtieels.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gtrmdqwzq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gcidzuurc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gmhfpidwt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gajvpltqw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gmypqsjsi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gcngskjoy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/garnllfnr.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gmxqgmqur.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gchqdwewb.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gyjiejprt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/geteymipw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gwzgfeefp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gaediyymm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/grhecpjzs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gyvxnsnoh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gghzoleqh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gdevuyxbm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gemwjdgbf.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/golopiolo.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gvojfvyrr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gnkmdxara.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/guqgozpcz.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/ghwkpztzi.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/guotbpctz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gobdfbhrj.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/glbjmqagn.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gupnkuojp.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/guhbeeuyq.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gzhqyksfb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gjiirvvcz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/grxosevyt.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/ghoyncvol.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gszsfqpia.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gbapiptbs.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gzodadvrf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gzsqderub.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gaadwjaco.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/goffvklhr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/grxymfygq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gqdbeibrj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gqhwhdxcx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ghkqhvgaz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gqumieokk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ghmfrrqqz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gdydflgzi.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gxfzxvzni.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gprftowvp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gipevxhwl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gaxcefoeu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gkgtermgg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gmgnorwtv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gilqeeizh.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gssefpiag.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/guscrasld.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjkezulfy.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gjxhwulzh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpeuzrmch.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gsynmieru.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/ghcgsnwtf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzhamazdi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gquvxsrss.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/grovcnvsz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gcnwjfgqw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/glzluikof.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/glppuxkme.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkcthxaiq.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gomhoygcn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gdrqdcixr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gqxsuarhj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzyimtsxz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gdcxxjnlb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/ghirfrchv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/ghjcghsok.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/goobvfybv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/ggbjooxys.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gxxlemgww.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/ghcwcbifm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gyysgokkj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gowysnghl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gegrkjtbf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gpcqtdqoi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gordxpfwo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gxrngkpql.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gpatbmwng.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gpigxthfb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gdkrnvfmo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gisfuufdx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gdmpwmaxy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gfiufhqkd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gooyhsqtz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/guobbrmyo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gehlwycfk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gddtmxbtt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gemstngkm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gylzhbekk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gedgpnfsu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqkfpuhlt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glukyjwhy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gjzuyoeze.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gdclpbzxm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwokbtrqu.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzaeqxspv.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gymvqclei.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdjweafxi.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwchbbzfh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghgwjnfso.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzrieqgcd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gdmpejtqu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghcypzsol.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdrfxipcn.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gwabrllaf.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gkztwadgo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjmjcvox.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/grkagthsc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gfqzdxgav.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gkibltlcx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gkkocwzog.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/ghgpyhopk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gbbguwxgy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gpsgsvcsg.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gzgqalowb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/giefpuwve.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/ggpdoqxph.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gfgqeeusd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gccmmaiis.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gwyxhcvbn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gwxdstzbk.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gltpxheeu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/goejkyxzh.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gqqzyrdwe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxlxxdwhl.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggcyrqufc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gjswajefx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gnavmttxi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gzqcmxqoc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gaemnlxiw.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gushcxobz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/ggjfzfwzx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gqititsjv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbwbqsxxh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/goplposuo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvyiuvtgi.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyziiinwt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/ganhcpgiu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gpwyoeiqx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/glbdrwewh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gefrelycs.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gicizhsih.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaojiibbb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gqiaflroq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gerjcdluy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gaiezvclc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gfdtrebbs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/ggnaakyrs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ggfkbtflk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/geydcdwal.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gldkmcqto.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gerehpaqa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gnrfsxuwj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gmcluwmxh.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/genhziqov.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gbgucfocj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gxhhxrjtr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gnssebjhc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gvjdwxmpp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gukocangp.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gqjyjzstt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcaycjrxb.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/goitqvpmy.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gjvswpnow.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/guosnnyvr.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggyoeljnv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gfwimshcl.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gipjucxwd.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gmcojhojg.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/grswuyitw.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/geoxquvda.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gwyqkdsgc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gqmdkyjyx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gwuyqawnr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gwzkhffyk.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gnkpltcvm.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gjczcubux.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gaakxxbom.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gfmaccbip.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gwlwvvxfz.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gvuinvrks.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gzezduexa.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gonumkopi.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gfqbaacqt.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gpdorxcns.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gdzptlaqe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gwyxhojdh.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/ggobauhug.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gqmdhofqc.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gijznrfxp.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gxnnbrxwy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gmfcpzwsv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gpaqkfdik.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gdeipphgb.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gweeerqhj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gtevxduge.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/guiggfsje.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gbslkjgxb.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gaiewoqmp.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/grgxormmt.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/grarzuwxd.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gvsilzprf.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqhkjhfmg.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gkrxbcoww.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gwrhfyikj.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gruouejiy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glywtquzk.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gudqbdlop.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gmbdvuwsk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gxolzxhzy.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjderveik.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqvsmjcde.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/glzqzoffm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gvyfwqgxo.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gatycbtgx.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gwiypldgv.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gpnblkggm.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gjfwnwemk.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gimemzfwx.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gstxcsqbu.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/glrsvhkfs.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gptxadsum.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gthtfinbg.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gpfxadjwa.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gapujbegl.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gflbfnwhm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gnbrieflt.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gqkjdovwc.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/ggtlrrphe.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gkgugsovs.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqrpgtzvi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gsldkdjts.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gnglyfspy.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gmvgyghkd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gssujhyfo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gtvhepcxl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gagkuobbk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gtbhgbmkc.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gqqxmwsul.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gvkrbzbdf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gztqbwtin.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gpaxujfrp.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gvciolfco.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gpztoyzxa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gtpngmkjw.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/grbpnitcw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gqrfwlhst.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gvjtwuaao.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gvxzmqjyz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gapjxweuv.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/grrkxwqhf.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gvjghfomo.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gfvgmdwhn.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gitylhcfk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gtzurxznp.sHtML


<!-- 参考信息 -->