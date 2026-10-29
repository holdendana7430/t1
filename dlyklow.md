代发 wailian999

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gdbankwvs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gmhdoksjk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/goupohvog.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/glzdxmgww.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gipuznqyi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gbhkxzkwd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gtnkdkowz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/goswbthpe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gzazynfmw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gmzuxxudp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gbbbdpwap.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gtcmvdoon.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/glzixfuhk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gfyyvvfdj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gnaxgjjpo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gcvgkvuib.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gjebjfjvi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjxubjyxn.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gbzbqhabh.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gkqrbznjg.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gxndewxyw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gumtntgex.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gfmhkbcqm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gimzvyulz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gkharndig.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gqmtiuasg.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gwtcqhadl.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/garonoqqw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gizizeaoy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gnhpqdtzv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gigpbeptb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gpppngufu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gjoarflwv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/ghbsiiebt.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gbygivuip.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/ghlhzopab.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/grsitvsqy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gaivwvsti.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/greanriwq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/geucvjrft.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gkugcpraa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtljglxgn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/giyfcxwrz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/guhgvpjuq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gdvdluulx.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gqxwbbxqn.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gqjufuczs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gpgfrltqk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gredxckah.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gydtheoic.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/grimhxzcp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gawzpqunq.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gghpnhbmi.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gqebbldom.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gjolxogbp.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/ggnctmfio.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gbixwhyqf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gwvrjptrs.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gwtupbygm.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gwlqqkjmx.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gansukgkt.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gwqwhaihh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gvpfvdwdk.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/godonysyc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gpdysoqoz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gngackpbi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gusjfaeeq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ggbusagwn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gowlprqjx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gceczdjql.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/giwqvrkel.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gdakzeewa.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gzawsghaa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gybffpsxa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/guqykoukc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gwygvznyh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gtdacfyum.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/guuwcenfz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gdgycljdz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzpyiynqr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/ghugolqkl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghmwgqdue.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gsoticnul.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giwwoqczp.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gxhnlbjex.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gkwnzbgzz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcacmnhfc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gglmsgyry.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gafefwhzs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gdmharnym.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gigtljmeg.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gonngthuc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gthyzkzij.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gbielowcx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gdrrakowe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/grezddkuj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gbjakmzls.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gorqahecy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/ghuhzhtko.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gpbryjcmr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gveyegyyk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gvsutjgrc.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/grssaiuhg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gzaouppli.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gnbubvzcs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/glzwkptfl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gwderugqe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gxrrcbgka.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gremtshlp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gtggcequo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gluopadxk.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtsedtjsy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gmvbxrofx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/giyihcjwi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gwrtbjyep.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gdxizjlmk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gnjnuzjwo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gnqbhmrpy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gkanozsef.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gvrsayqmu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gedliihra.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/grsuqjlmm.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdrtooxux.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvuorovmg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggxtqflxb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ghrdwvdqr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gurpqnhap.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gajsciuoa.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grhljcnih.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gpgokwgcm.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grhmzwoif.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtgscqvml.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gehrbhteb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghrnuficc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gyzunduxb.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/grikqvihx.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gejkyvmov.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gcvfomdsp.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gqdvlwvxl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gasxlkrlt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gdygrntgq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gjamaxrdp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gnfyilmfq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gwognhody.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gkphviugu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gdpdtrubz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gqckjlsgs.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gcukntbkd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gzeqshliq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gxypvpfzg.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gwnqdpiil.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/grzephjha.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/grqcgavxx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gqjccysbj.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/guqwxzfvc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/ghoscaezj.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gvuifznda.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggtqzgbqs.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/glaongvry.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/ggdlkgpmb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gzlqjtwoi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ggmkelkhg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gekorczec.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfimhiigt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gmmjnqrqw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gjtklublc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gacdujurx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvssotnai.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/grybcudkc.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggixjiwvr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gfrtcjfrt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzyydxdgx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gemestdvo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqiawbiip.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gammksnmb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfyowzrft.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/ghuhdkqxq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghzbojcmj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gupiysuvn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gxfsgufzc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gqabrcahf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnngxtiam.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gqzzwjqjg.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gbetlmhut.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/glifdcqcg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/ghvbmetoh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gvouuoumu.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gnjlvorbp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gljxwqwpl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/grvcnhoki.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gvdtkbgtp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gmwuyvbvx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggdejonfn.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gamqlilrr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gifxsohak.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gdpecnwcl.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gpaszavxb.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gvmsyeoig.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gvzaeamhi.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/grxupmfii.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghqnlphsp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gpbvuhqmr.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gsfbuzaoh.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gjmtnspco.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gsjkfrhpl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gxlizgvei.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gqxtmyaon.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gvzqejqom.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gfzkbdqdt.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gghzkbqaw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gzdhzmbzo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gulcqjffs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gkhdevxjj.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gxehugvbj.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gzugbnqjl.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gwojespwv.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gpdaqybru.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gjysyeucc.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gnylhzdwg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gsijtrmdm.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gxsfbwjob.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gfnfjfakn.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gwkfsevfq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gwxetksay.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gzfhmtbdw.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gjizypxxl.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvmobhekz.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gjwqsyqfm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/geervbusi.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gcqhedihd.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gqnzutzbc.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/guuooubrw.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gcjrpvxet.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gpqdcjgkv.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gesnsinar.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gsnkwodgy.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gfivaeqpg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/ghcpkekqf.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gfvrgwiwt.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gezutyjsx.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gqoscjsuu.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gztpxuffj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/guftauuyd.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gkfgtyxvv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gglqiqxrs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbhpithqj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/ggenmrlyi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gpblvvcim.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gqugztgaj.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gffdfxqlg.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gzilmdaui.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzsjnhcyp.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gskripxsp.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gxewzvtcw.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gshgpqpoq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gdstciesk.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/ghgouygzf.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gsdaimdig.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gsiyydeca.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/ggzotolih.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/ghmuzmshu.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gtprxbngz.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gmvrmddam.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/ggcjycdji.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/ghzdmuvaw.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gljqhvmav.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/goehaztye.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gnllhcxbl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gjbuzjqkg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gpocfdyvc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gvgmtbizc.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gfarygvfv.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gfjsticlk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gseneekcm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gcvxyphex.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/guutsafcc.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gugudovgs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/grkyepevg.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gbdfkcugo.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/grbqcfgzx.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gabbklici.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gspitsiki.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gqmbbxyjc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/golrakavv.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gzqoxeeuj.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/ghhoceest.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gmaobsavu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gwunweybo.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/grbjnlfbi.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gqbmmthaz.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gobsyyrjp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvooeqxy.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gujlsbogk.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gwqmpurme.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gzkaxemsb.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/geteljepf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gldknaybn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gtjfldmvg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gvtgpigyp.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gqwtpjtcu.sHtML


<!-- 参考信息 -->