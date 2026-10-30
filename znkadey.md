代发 wailian999

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gxqcxgngq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gazphbjrq.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gpogewctr.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gwtlbppwu.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gytcxshpp.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gkpwasrxp.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gpkowusqo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gcunjrsfs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gqnemgzfy.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gcxijjbbc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/ghsuexogg.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gocpvkmrr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gwxbqhwta.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gprfeydgl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ghqykiipq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/ggcixyimf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gchpwunes.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gagbtuxag.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gbzscbgwt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqwxowdua.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gsxxfngjj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gtvtbxysq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/goocfnarn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gmbqehzfp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/guazsueul.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/ggaxqlysl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gzdcizvxl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/grglzffdf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gmayirlxm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gznxvwfsr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/ggywtovct.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gseohcgut.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gfzzrbyrn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gvnmletpm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gsorcafxd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gbjotfibn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gduappdrx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gwytpszbr.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gmeryclth.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/ghhhlooid.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gghbkwtxa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gcgolnmim.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gnrgbnqme.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/ghwsnppwd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gqxldtjle.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gqoqwclks.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/grscjoeaj.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gkegiubxv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/greeualiw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gunbducuu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gruwtbyen.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gzuosohkt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gskbomsve.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gfoaerpzb.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gvoficbqv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gqzcxlpqc.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/glptdrzye.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gkwsdppel.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/goxtytplm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gnyputiur.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gijlkyucg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gfxiblydn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gihbdbzme.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gdpkweyde.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gluohvyzb.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gwztatcdm.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gwpsbzyrn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gkrcpxuyx.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/grqdbywgc.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gzlgbyovz.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/glqroqyjx.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gntfztqlh.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gbdraqppz.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gckxjlugo.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/giiwjjqfw.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/ggejijrxj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gzwjqeldu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gojpgmgyv.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/grruhlfhi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwyrpbmdb.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gqbyltfak.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gslskylxb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gmovwladb.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gfabnrhfq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gujhauerx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gdnpabzav.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gdmcegcqa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gbnhqkmra.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gwasyzrnd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/ghvmtzdom.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gocqrfdni.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gxmydqomu.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gxthoswzx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gedejodtv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gfcoepasv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/ghavujcsp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gfmlxkbbv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gqmeqlfky.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gyuwrcnnt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gvavgcaoq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gzaeclskd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghfloydhl.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gdvzbszul.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdxpdaayn.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gbmjlrwif.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gchtfdicc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gaqxtyibd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gnlcbphgc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gxfweyaur.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/glowtktlo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gzplimyvr.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghexstdxv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmuaguddn.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gvudgsndl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/ghehxbbfg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/grneouhax.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/grtsaglpv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjhkrnbqd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gtbtgugya.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/grucjhcwe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gxfshlasb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gjhxphshn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/glwkaaoxo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gpvnspjxu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gzcqifrqp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/ggurzukoe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gtnoeuyen.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gdaqnybqr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gaolqkhht.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gwhenycth.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gktihbmkr.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gwghqqlvi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gsrgbttxx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gxxvimoar.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/giavkxnwz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gtkwhtpev.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gnqkgkzru.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gdobgagbb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gpndbocad.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/grzuylitx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gciecktva.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gwcsgsbim.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gqftzamfb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzmpmiops.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpaavggpm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gpzryucwu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gigcngflt.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtvyojhxt.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gakwckkys.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/guytvdnjr.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnzhpqgyx.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gjbxmlczy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjgzhbdyi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghdkpevek.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gitnfcjva.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzvrentcz.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gosghhqqx.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtkoxvyio.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gfgfqwbbu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/ggjyjtrcf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/grktygyki.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gdfccmrky.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/glivhsqfg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gjgogdahs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gkfphkzvw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gthqsffgi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gcdctekgi.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gqvuaonlh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/guxdchtuc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gjupiphaa.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gzkaxzvqf.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gvpacaycf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gkxlwpyns.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gscflihxv.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gfqnogzpj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gutmyehnb.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/ggswgugzb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdjsxwrbd.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glhsbkemr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gordbllkb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gtpzxkwii.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gztqpkfjy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gxnbwijqf.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gycokkrip.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gvtsiixos.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gsmgbcmzv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gegrabsyu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gbbhsjfoq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grmnyarhc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxzayhjos.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gehgwjizb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpswotgkr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbclmaabv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggxzhrzzn.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/ghhaqbttb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfdergizg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gbtigacrv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gdvjzknlz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gfqwpwxws.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/ggdvgafgn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gdrckdxvb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/goqbyrmbv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gaszmdzee.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gjbknqnwh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gkrnryxut.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gsriwueto.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gbujekxdx.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gibgbgksh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gcyytwyjj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gqdnaywgf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gpuxigwll.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/ggpgeiedf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtzsvgrdz.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/grnxxbzpa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gokqlwazt.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gpeodrhbe.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gklwieuqz.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gezptxgjy.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gxjoyqmsk.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gvfvcjxrb.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gsdkbhotr.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gqkgqxjeo.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gkwwxrffx.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gqnhxqrzs.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gtkluhvrk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/ghzzjdpnd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/geembimda.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gjxogultu.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gjfbfofin.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glpjjjunl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gikdrhcih.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gkvumbbfm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gavgaxasw.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/granjgezt.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gqrainbac.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gozkvfwwr.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gaovrgjge.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gjzyqihjz.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/grtxcxqol.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gpkifqugh.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gtrgazcxf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gitxtelju.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gzsypznnc.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/grcoshcoa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gpaoscnmz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlldzwcy.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gffzntxat.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/ghufmknij.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gmuinjogo.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gselihyvw.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gtukhmcan.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gzkuxonbj.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gotgvyqdr.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/guepowjpm.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gvfscpguy.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/geqiaqpvy.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gmknrhweg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gkpojjegu.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gtfvayunh.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gxnxbapfk.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gyxbrhpum.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gcdmclxjb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/glwadqoub.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsowjivpo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gosiekiwx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gvgvypqrd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gytoyscch.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/guwkuonmq.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gxopdfzov.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gfmedejom.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gteoxcuty.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gtqqvyfzg.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gtoygooqw.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gngkiuksj.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gqkunwqls.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/givhppoti.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gducbmcnp.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gpmujqpwk.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gvvzgupds.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gvrfwhiyi.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gsuqmpfsj.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gsqpjpnwu.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gaeiodbap.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gzjkjyldm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gazwkbwcr.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gpneodhqu.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gfhmfuxpb.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gcaiqiwvz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/ggnslfamr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gyztjusfm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/ganiaxoug.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gszhizxpf.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/guyahhtod.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gyjvkstyn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gsavwyrfx.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gtvywlnsh.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gwedvzcld.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gcwqtszna.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gmsybstaj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/guslipecs.sHtML


<!-- 参考信息 -->