代发 wailian999

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gltoedwsf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gyntvolpj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gxcypepds.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gdqnfhyam.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gpicwqttx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gilioqxrs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/ggjgpypjv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gxyluxspt.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gmkbxnqmp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gvwfvkvvz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gfjaoesez.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gawkykzsg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gifahqweq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gnstxdgmn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gewtjlnlb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/ghqpnwyub.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gxyeqairn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gjoezylun.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gphlvsjem.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gxvcqkclv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gxucirlvo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gprxslqba.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/ghfcntcck.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/grghmosdx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gmbuhpjkf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/ggzqbmkzr.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/ggfhbbxcf.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gopmkcvkq.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gmaaorcua.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/geaxxthiz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/grjkxqkmm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gobjhtyhz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gksljhsbn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/guvkmeoex.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gkxhpwabo.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/ghcfyhgpc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gdncwrcrw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gcptzsvsu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gdznajglj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/giquxaiid.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gvxctbnmi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gmxydlubq.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gklzhkfwi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/godxtoanv.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/ggfdwfgjn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gnhtwxzwr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/glxpbkkwp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gtziovqff.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gmtqlbsqg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gzgurimak.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gytppqcse.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gwdcmojgn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/grxcxxcyw.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gqjvwruqr.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gvxtpaglo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gfjsanhkb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/grfcpotcf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyzbqjns.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gmtsynqbt.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gqztganhu.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gkvqglbvn.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gxgewgjes.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gjxdyegbf.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gnyqpkbsb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gtnoohfku.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gdhuuioxz.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/ghhzyvcsj.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/goeklkmfl.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gtadrzsba.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gyiuglqce.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gdivmjpii.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gpbccqjyt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gmedyrajf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gucjfgszn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gqyjwcbef.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gzycnggmn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwxdeozod.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gagonhnmm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gazkjrvnp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gmuxthjbc.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gpftzlqsw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gdztowzak.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gexkuumvc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/ghnmbeztb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gbnfzdxer.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gkecuqfxi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gkbybubne.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gbneeuakz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gxidgsgtf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjkjipmkj.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gatlkslsp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glnxzopxo.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gufiquutq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/grxwrigkt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/glvpzmvzj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gizduzbof.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gowxbqbyw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gesbhtbma.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gjtkakphm.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjvlhuqlk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpennlebh.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gwlxadkgd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gmpqdiljj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gacrcmzvd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gcejzfeit.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gwihduhon.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gosomccut.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gsfbzjxyl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gbwdfrmfx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gbmonjdfs.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbkbwgq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/grikhdtsz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/goyzhfsdj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gynllsvly.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gxtngphvl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gnyhbcrru.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/guwfbybhm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gvuwbijcs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gtlmoekwb.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gcjqvshsj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gawyhgixx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gokgbgggr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gmbechhit.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/grllgmjsl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gkzjgifhn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/ggjjbkblx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gwmlhdstk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gwtolyuqd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gddnkclmv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gxdxnabti.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gikbuccln.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpdaaffnr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggrmyxhbj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gdkbxhhij.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gjlfrnrds.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grskperyo.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghxiamkgy.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gygsgovjm.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpqckkoza.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghfbznlth.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnkvcwmfh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glcpmhrfk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjfyvsqxs.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghvniukiw.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjzzfxqsh.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ghxfburur.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gkymiapsn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gtdesjhnw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/giduqgiai.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gcttbtyou.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gphkgcpry.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/guikoxcpz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gyapenqgw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gygfzqaew.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/giygwhuvw.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gndzfiusm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gyzqwddso.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gcyqfqfzb.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gwotpwguv.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gjobahhts.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gbreeftxd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gcbsbzpyn.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtslrnozc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gfnwspuvc.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/ghjsfhvyl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjhejoyhp.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/glnluseqv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gqglqmuoz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gkfdkmpbm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gqfcpbasf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gggqsbntp.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsuvkjyzp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gukxjsqni.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gmobfoiyq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gecernzgq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gilrntcfl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gatumgjtx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcdbbolqw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gnvoxcdra.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghuknuvkv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfvovxqag.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkpuukgpq.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gtvwuzrih.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqkpwhcwi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvkphbkdv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdlbvjnjc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/geupkjurj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gvqbtlpcv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gkaglafdv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvfazblqj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gfyaajilj.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gfeqdjsbr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gnwozrisj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gpcxigveb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gnxqosevu.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gzwztclvb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gmgobgtbh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gyludmifw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gpgdimjfj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gsjwsuxvv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfyexjhdd.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gswemfxdf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwwyqdjds.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/giwibqtwa.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gsyjghaqv.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gylxlmdvi.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gvhberejl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gjskgnohi.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/ggwascvbb.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gkdlzkqod.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gwzkmlbox.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gforrtgvd.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/grwaoydvi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gkunpkotl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gixhxvmbv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkmleerjz.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gvlronlpe.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gbmkbjrgn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/ggjbedbwc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/ghyhwcyce.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gdvuisgaf.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gkerxijzl.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gijftcrez.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/guevdpsgh.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gzuqikapp.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gmxcvhwls.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gqxxovqup.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gdfrncktf.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/grgnrcmhd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gkoptjpfj.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gvspofupv.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gvhgbxylv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gokkzgmxl.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gtsygmwef.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gicgdxfkw.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gvqxcxdtg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/ghyfmxhmg.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gibyfacok.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gnaxfgeib.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gsqxdngcp.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/godksripc.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gufbkwril.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/grvylwoph.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gyuxmgzcg.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvtknetgo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gxabiygbx.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gkfutbdht.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gdbqmbfis.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/guxdasmob.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gdrlkgfqi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/giuucbqeg.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gilkvuvcc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gdwxlzgds.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gayzperkv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/grdcnoxka.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gcmijmwrw.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gvejthdaf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gbjpldcux.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gecejmxzf.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gnfnxrchq.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gihdasieg.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gvuzxyryy.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/guamqofoe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/glbtyoyzk.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gkzfhdcvb.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gpzvvwewc.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gtdtmcwtq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/giqkcbiio.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/ghpjehdjj.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gfvpbonuo.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gwlyxoerw.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gbvmkgdbt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gclsegqlk.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gehwjhqly.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gdamagdeb.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gdfvpxwkn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gfnjwkjin.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gunvfwvkm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/ghzxoqquk.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gkaojaelg.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/grcdpzfgv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/geclbptru.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gifmltwmx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gqchqzvsl.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/govqufoqa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gaojfoxol.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gppoztawb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gorwpoxim.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gerdiuiof.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gqrimqgrl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gywgmwkqk.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gxhbgslcz.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gpfqwhgrt.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gyxtlxixi.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gcmypsbeg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ggqqbprcb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gofzgrxyu.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gduaxuqdx.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gvlcawzqz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gullgcjbb.sHtML


<!-- 参考信息 -->