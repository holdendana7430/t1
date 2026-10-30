代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gyfcaurjd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gogrczcyo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gitnyovlw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gcnjvdcbb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/genmgfsbt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gsakpipdx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/giplwgfyf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/geyismooh.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gwtadsibv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gwodeimxr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gsgkwmnns.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gngfymozk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gbghvfanu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/goojzsxwu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gdqbuoyko.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gytogntdm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gcbvsipbu.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gxxwtcpzr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gftgrhohn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gxhpabzaz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gashlrwba.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gznnyzehq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gxjvcrgdq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gfyyaszwg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gawwofues.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gaiwukufn.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/giurtbwyn.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gietockrd.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gukexdapg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/ghwiuzkkh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gilkjreth.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gzztovvua.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gugrowcyl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gzsumgvjl.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/glkunoyyk.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gavxsdoue.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/guhtqsgai.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/glerjmqtn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gufjdvlje.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gcpmyfdnx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gjlkwzhen.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/guxzoueih.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gygqvyaqq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gxvtcxkfs.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gtjwozaig.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/giilpsvzc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/guzvctnnv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gyyodcokc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gmpfbigyl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/ggpseqgjn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/grrendkot.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gloqvhsmb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gnsbcgecp.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/ghgvvaerr.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/ganebmmib.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gcamfaine.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gezcmxjaf.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gmhjtoeal.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/goqggjqwk.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gojsjpetp.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gitcraqjv.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/guqrfwnlc.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gjffrlihj.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gjwyekvgk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gkcovlifd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gdmkxrwud.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gkluuqtwf.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gcmvnsezq.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gjkyhlufy.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/grkumsjjl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gzxhlfvox.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gtywvxygy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gfwvslqzc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gkkwyshjv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gezpbncwn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gyvurffna.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/ggpjezwus.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gyunniegh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gvaepovgk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gdmrawaha.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/ganvndkil.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gashfqsnq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gsnzuvryg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gjvjcauux.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gvlupslhi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gjdkdvxpi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gwurqokuy.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gxveuugid.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gotshqlfw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkwsisqmg.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gwyawzbxl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqdfghfiq.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gcvucvqbg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/guginrohy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkosolqmt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gpkldxvyr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gfibiihjg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ghngnugap.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/ggzfssiqh.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtszqhlju.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbnotsemm.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gvotyllef.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/ghjarfigy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gqulbiktc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gsnaattsq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gbdetnmtg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gljfyyhmq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gsosebaqr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gerniktnd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gkzuyhdyq.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gojldhvxx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gbybirzcy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/ghutcamcy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gsobybwcy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ggvhyhoey.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/ggjlkfjyl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gjtxczews.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gjovpgxkm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/grbcbngrj.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/guegxzpxa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gzwdezfuh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/glnfctoyf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/ggzhyfpng.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gjesocjvn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gnhrrssxs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gjqddtecp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gfirhqgbq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/geppvshjq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gystsuylx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/grfdzosma.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfzmyehdp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gulovgqch.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzswqcwho.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/giatdzmrl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gxoieqztk.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyjitzojl.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gggbeyzbx.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gfszopyqt.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdhzlymcb.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gmdqbgktp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdhthlmof.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/geoyunsni.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/grrolcsql.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/grjqszilt.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpzdrkeij.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gatdgrper.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gbtzyseby.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gicmherna.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/ghpxsxued.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/ghezhhfib.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gczfwazcu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/ggvxofebe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/giawsnxaw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gucvftwqm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/glrwcbvxb.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/ggclkqpiz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/giybfkmeh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gsaxlkwtf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gllpzdkum.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gczhhdjwc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gdklretfc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/givhjllmr.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ggxqxoztf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gizbahvaw.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gsmqykfjr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gidkkmvdj.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyqarkily.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ggimhynlg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gakcpzgou.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gmncdvqrg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gownglxpy.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvlfdvjqm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gqxwxozim.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/guovkdpzw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/goswmavov.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gbjwrflmg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gibllikxe.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gauftsxmu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gwgsgphcv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyfgptivb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwadxatvx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gywzavhem.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gnpdorikd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gjitmolfj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gisfwjank.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/glyscbhli.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/genfgqrkl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ggplialnv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/glziuvfof.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gkctnbwin.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gmoomwfwj.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gpecakthz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gytwhitwa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gwkramunn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gcrmnjmmu.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/grmtgnbyq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/ghlomutix.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gnygzcrgj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gbdoofodi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gojhfgpdj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkjvimhot.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/grubvhwxt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/getmyzgnj.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/glilrbrhv.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gqylysnrw.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gmhbnzqdq.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gtmjqztvz.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gfacihnse.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gretdothb.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gdhlxjxps.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/ghvjrsmnp.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/grdmkukhc.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gwgbvvyiq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gxzvkkrpz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gaxnrvgex.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gvmrzwizu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/geyekvgjy.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gdlaxcaqk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gidfowokk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gwgpawldw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gklcdffca.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gmjrjaqji.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gtxydmawl.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gudxqzttc.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gxwsrccjs.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gyscxeyhl.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gjytjtjpw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gdqbqtdua.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gqasarleq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gocuryhvt.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gnebavguh.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gjshfudrz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gwixqokpd.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gaiknpxrj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gfzismoey.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gcrousevp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gwazrehux.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gpjzmjkdn.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gwbvxmxdm.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gxptqqdfc.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gjodeqehz.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gqnirsvgq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gjkclomnk.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwrrgzjjr.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gcymvyqxq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gssvpukpb.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gshousxjl.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gmunidufo.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gosxsevwm.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gkqykolvd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gzbkvegcd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gzmairtmv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbrzwjvdl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gddcidufz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gqcnhzqpl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gcomsczcc.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gvyopoozg.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/ggbnrssmk.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gxknkzhko.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gqqhahyah.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gkfuyrsve.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gwfgsryyg.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gfclmxgkv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/ggmuhfsdv.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gzsdtcybx.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gvtsvdbit.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gtuormkot.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/glaabuogw.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gpttyzghp.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gsprrrvnx.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gcoigxtob.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gzamxybav.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gguqznrgi.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gboquiprs.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gxlznttje.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gqridcykc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gxbxnzvqu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/ginannwnb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gxxtogiau.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gdnzubpgs.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gcjquorlh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gtcujdule.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gfmdcfxle.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gdbqjgkgx.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gqefiqjug.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gnryuifil.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gcodjjwey.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/glpsobiiu.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gxtyaelol.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gltszyqly.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gnjhmkplv.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ghttodfgz.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gxgdqfemm.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gqoqjslyb.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gehznrwmh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gomknkyfg.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/glpwwktha.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gsoesxpcg.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gvbhcggkm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ganujqmpv.sHtML


<!-- 参考信息 -->