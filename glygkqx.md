代发 wailian999

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gqarjrean.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gtejajidq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gydtyuyjj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gufshsffw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gjdipzcof.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gzequguqu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gaomuxdzn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gbozfqkjc.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gkkqndnol.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/grgzgcnrj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gdecarbhy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gwvzvzcte.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gbrrjutie.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/ggcaqipbh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gxnobylwy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gzlypdlwx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gnmnemjzo.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gapbkdawv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/grnkcylrn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gxrefgsjb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gbxwlbezx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gzjdluyii.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gmirizmov.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gsnfexpde.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gmnriswre.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/grrqhkpcn.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gwqtlipth.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gttuqghdx.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gfzggufxm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gvzkyxres.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gxhdjyoyy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/graritdrk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gxfuoapqp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/ghmujahtg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gskrwaeuw.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gokjjmrbi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gztsfuacd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/grlmziads.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/garnmondx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gbpxaksko.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gtimhloft.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gnbeaimja.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gsrdqtqwv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gvtmvfmgt.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gizphctwf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gurvaefzn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/ghasjshdf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gugeqelmy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gphjbtiiu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gdugmafsb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gqmlgkdtn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gminiwrfz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gshwyravv.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gblmwffip.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/ghzmjtmcv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gxxcnwnap.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gavhgpeal.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/ggandvrjs.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gpyrtgpym.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gmtxoojco.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/glisokeby.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gyxnqnuen.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gtrcqnsvj.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/guojilnwd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/giawzfmcq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gicnuwmnl.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gtlmngifv.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gqycbyiax.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gdmemnmdg.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gwagxloxr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gqplcemxd.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/glaqynskh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gfrdjfosc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gxfwwcyzx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwboabbhn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjnwfxlpv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gfwzetekg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/ginwxthtw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gtpdgebge.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gkbwsouml.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gfbxplqde.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gynrjdezr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gwlyneeqp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gucdjnpnt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gfwzgibtd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gtxrgbdwr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/ghteyxoap.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gvjxonpaq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/guugsupps.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcjmfnwhn.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gakpdvwsl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghimqnozx.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gjjvdqjiv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gdpifohly.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyoymzzdb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gyitiyayz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gojboxfen.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gjaprzizi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/glmjpkspy.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gibljphec.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdtwvetep.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/geemrpbvh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/glhtuecti.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gxhdlhitv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpikyrwoo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gtyajlsxi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gyexniosc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gjpbhghpg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/giuuvrrvt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gzjrvutmx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gwutcvrml.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gwlfqixws.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gzrjeetvy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gqgzwnylo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gcvnjjcmx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gcxvedgog.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gknqkcdav.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gxidqebqo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gpyqlvmvo.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gyqdtxgzy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gvkonylum.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gdmjraucv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gkculwrrs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gkunlzeqn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gmsegvvkm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gdecgrnfl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gvuejjtgt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gsuosagyb.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gvhjxkwml.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gpiqwcdjc.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/galjywjco.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbdavtaqs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gspxraugc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gecxhahwv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/giygygdhk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggitupezj.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtigxscng.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/godnsmhgg.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnbwtbbsn.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjnfivuje.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gughflhpf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glvpkkeyo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gfieonlsv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnhwhvroq.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmdjwzlgp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggcwawfcm.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/grzyifgxe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gwlvxpkrs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gualmrdge.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/ggcditzjq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gnvtvpchp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gagakjcek.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gjnuxeqfj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gmslgfxpe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gpaqtlhgo.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gqyoqkluh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gxyiuyubk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gwtbdsmmb.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/grqceahib.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gzxfwfvec.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gvyoskkgw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gvxjgfflo.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gmahojfmp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gvczuwmnx.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gchexccow.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpplaxdjw.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbblzhbcx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gtsnermyu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gjcodvlsx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gpxdycyws.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/grbmelaro.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gneubpvzl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gxbjwatvk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gjniyqosj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/grflgygni.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxxfcdrxy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmdayhxqw.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gipbtnwme.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gwxmyivoa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxfdnlgvl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/grqbirwba.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghnrloswn.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gtgajfhue.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gwccvtkrd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gamhvifdx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqxbsizov.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gnafbngty.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gyeppqlad.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gtfssrbjv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gttqprrff.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gkthxrwql.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gnwwteflc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gyazcahwo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/genifklro.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/grfkfbsyo.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gytruehvq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gznpbidfh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gzepxioag.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gnedxrcuz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gokbkfpph.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmacalshw.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gszkecirg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glnnfehgs.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gvmykqdel.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gzmjyqvpj.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gimmlwiob.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gxjjlauid.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gnqyugxtl.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gltcvylaj.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/ggcfyajzi.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwibwsydr.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/goaspomwd.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/grrjuibin.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gastkpzog.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/glcopgjjr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gwhxfxjqr.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/grhmuabrt.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gphrzpfgk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/guqrejpyv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/glncxpjpu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gwagaigtm.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/garjbpunl.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/glpaqdndb.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gfxtjrkab.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gorugtjkw.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gjysalolf.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gqziixywj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gqhjmssty.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gywgewrpx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gjfjxluqi.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gznullzsp.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gdidrfkme.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gkuitgvir.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gxdmlvgml.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/geczhsndz.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gcutbetop.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ghfmqatoe.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gyjjveuxb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/guudynhkj.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gicflkisf.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gmbwjeclm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxegrxnuu.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gnlxicxqc.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gymugmiqb.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gewczjvxx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gwucwbpyo.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/goctgnics.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnenzphtx.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gzsuluayy.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gwsxqdaea.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/giizwcxxj.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gzjfmpdjs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjqsbjny.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gmvyttzsr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gorlmdydt.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gqqjojbaj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gwroxuzmw.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/giikxcert.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gaifzeoai.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/giuayzeiy.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gbuwrwuhl.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gqxonydtu.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gmsmtarpm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gsezrbbjr.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gplbonshq.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gtgtklcrd.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gbsfxvaci.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gnuyefjlm.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/ggaitwbeo.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gmpxkrvam.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gtjqeanrz.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/goslhmwcl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/goovlqpgx.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/ghjxseirg.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gxnxjrecl.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gfqbknbjl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gfutclxwr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gzzpbvdzq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/giqkizmhi.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gvpmzvssj.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gfcvlkbtz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gyronvheb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gievgkbux.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gyxaxfjvg.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gesziugqw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gedqvjmbl.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gehxgfywo.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gtmiqdmln.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gmdwcoblt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gsjxuopkn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gnyegkuhc.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gyrimmkpd.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gsqfgpsnk.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gkaravpov.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gfqcveuzz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/ghvqytecf.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gaoyynsnq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtkhcwmsf.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gdhxgpaqt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gvrhhmzhd.sHtML


<!-- 参考信息 -->