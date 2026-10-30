代发 wailian999

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/glebvpozg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gngzrirjr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gqxamftqy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gcmmnodza.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gzafvtita.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gtilwyqep.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gkryjznvt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gtijxqpii.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gggoumkro.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gytkvairv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gzmbmauit.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gopvsqeje.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gmichzobo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gkuicmxpi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/guhxwwqxs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gezwhfbij.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gthlymgpb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/grsnalbkf.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gtdisrdnw.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gdxngujng.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gyuoduirf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gnbifxyle.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/glcglspcq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gppwelowf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/grquoezuh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gwkgcwgqk.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gryywuyfl.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gtvgenlvh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gqoguerve.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gpbisvqjz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gzubipcwe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/goemvagoj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gthkkumtz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gusprqplb.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gzsioasoq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gdzshllhy.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkwguxlgv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gglngjgip.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gqtcqjpxp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gsxkjgxdh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gnvzdldmj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gqizfatsz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gimunrwjb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqrajuimu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqucqwfpf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gzmalabxw.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gyhuaezoh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gdfedyfvt.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gxqlewrci.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gmyaadwzp.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gdqgrkmna.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gnigmwqfg.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gkerjqjfa.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gsrlbvbcz.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gwgmhocia.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gjnnpcdoi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gccudpaon.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gjzvhkxbo.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gtkqmlhoi.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gblxezjzl.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/guwootkqn.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gtwlpnlbh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gujdorsjf.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gladdmalw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gtmzeqxrr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gciuuvryb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gnqbzcmoq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtdmmwvgh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gyavuuhai.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gtqxxcjnk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gykdrzeif.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gztwfgwce.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gexolreig.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gmdcxuyom.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gyxmifyxq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/grbyvivsx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gyddjtbbm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gxolxunvq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gdmkqldnl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gvusyfxol.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gezyaggrb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxkfqwdyw.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gywpilvoz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghcztcceo.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gkytmiyev.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gvjteywro.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtoaieugp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gjqwgixlx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gjdhrxgsl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gxppdpgpa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gmbpejyql.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbsxsahas.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gywjnbihs.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/ggdlopwcf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gwihtxrgz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gizakhwcw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gkcnqwinp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gidobcqjj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gkrjlftqo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gzctgsiwe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gwszyyqgd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/ginvflwrz.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gminaqrae.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gdjrrictn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gwjafaywu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gexfzmswu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gecsvurun.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gmtlykbqp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gilbvcvkc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gykcfnklh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/glbpeiyfz.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/ggqpcmwhb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gmgkqlmoz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gohpcpgas.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gfeeqjwyr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gdcvxmsgq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/grhgsflin.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gzuodcrhr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gwvzipmmq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gfrypuyss.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/giulhxqju.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gqgyebfgw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gtbogkzbj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvgdyogox.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggjtontkc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gzsfmqioy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/giorcltuw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grtebolci.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqpnxytya.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/glnliymbz.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gympnvscu.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gflowvuqj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxftqurrp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqdwanval.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/geikctvjt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geavhiubq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glqivatwy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjwhsmwpw.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gtrcwmkwl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/grzfbzwbh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gfhydiyix.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gqvldcxui.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gyxuhumad.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gwewewhoj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gnqojlwkl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gingvgnna.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/guykgtuzv.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gqztndqey.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/giqkwhsyn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/grxwllnyt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gmycmrpkc.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gxamecqqp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gskwqcjza.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/glpcnzprw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gvanrxpkz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gbqljbqla.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gwrlfhucl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjqnaywel.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdmwrrdjc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gebcngtzt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gjdeeplxa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gqbtrehlj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gpyvhyqbw.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grfbpbivg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gfzvbzkcj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gahsikmgp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkojqgmzb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ggnftvmmg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gebltkzhg.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqrzvnawj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gwtmfbnzn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnxfrjnpr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gomhfeuaf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gysohmfej.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/ggsungkbs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdcnvnnas.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gawreyvla.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtrecfzus.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpjigfkdk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/grtyglkan.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gfnfuivjk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnsatyalp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gucdqqijs.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gnytgtzyf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gcdznvvrd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gubllxuom.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gxxlkpmdy.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gzbfvwjnq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gomitiuyd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gecnvjjkp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gtlilodid.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gxkebpztg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqipaqkor.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gpsjdwhbn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqgxrcjys.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gutjfbrpk.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gxksibqld.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gtyocgutc.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gnktpeybj.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gsnxssulb.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/ghpqbiyeo.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gqyjkcqrf.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gbrzksutz.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gfzqyhtfh.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gshhigakh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/glkjrnlwa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gyvpcdkhd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gvntltmbl.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gbvdmyhki.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gatduovnq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gxozadkkz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gwgxrsyac.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvcpbbmh.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gqlqcfwpg.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gfkzovwbh.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/grbcnszme.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gkhxmxomp.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gtqquxkya.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gswbdsswi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gpnrzoxpe.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gkbgyxiwy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gigqquegd.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/ghgnlbfpc.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gjzombvsq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gneiakled.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/grytrnecn.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ggceiapug.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gwailiwfq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gmadfjorh.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gyaeeexuk.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gluyyaamt.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gabhheupm.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gdkghfrre.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/grdkbnmpq.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gklgasqbu.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gwutzgtmj.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gcpmiwtpp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/grzpgjtwk.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gppdzrxes.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gmaqjpiva.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gtzhazcra.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gamszglqb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gmvkjdbrp.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gqwcjpxyb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gftygbfoo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gnmoiqvpm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/ggfintesx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gesswpxax.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gonklntdj.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/grpayzxzo.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/giejejupt.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gizruikra.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxsplgmyg.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gexyglmyn.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/geajmnnsi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/goryewfye.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gxdaqadrl.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gneoceqod.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gqzwkauum.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gimhdsrpv.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gtujseyxz.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/grwedptcu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/grnaavyar.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gvxuycite.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gmzfgtplu.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gmkhmpuug.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/grgjciyqd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gwolchcfc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gaeqtxcph.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gftcagpfy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gygijocgx.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gvnsfvipk.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gtnfatzlu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gsmwammah.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gygaiiaje.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/ggfeycxkb.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gauzmhnmf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gkfvlonhe.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gxetbmhuy.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gcyhfvcon.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gzdydlths.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gmtwxkumj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gfjfgljmb.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gldwspdbh.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gyzgcbygq.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gduclazmg.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gkugrczdk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gonhdvlws.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gcwtkhwqv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghvrfelgh.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gixmpfmab.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gyxkbstgk.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gptzvztvn.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzldigtjy.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnkjrfjgg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gonuikptl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gefbistxd.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gffmsutnj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gdflhcbnm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gdkphqlyi.sHtML


<!-- 参考信息 -->