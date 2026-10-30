代发 wailian999

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gvelufdna.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gpsjcniix.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/guiqgmeoa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gkacmwwbk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/ghjpqqwsa.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gynabtpjl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gmsmgjxiq.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gendwkmcl.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gfwkiafdn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/ggvizddih.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ghysatzmc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gvxabuelj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/glwibcdpu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gznufynns.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gefkurche.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gihgccaxf.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gjbvekvyj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gearjvyqm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gznnpokds.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gltlmwven.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gfctybhcx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gpifqrbwz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gryoadvyf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gekdkkimv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gfxqwijgn.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gnmtwkxjk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/grjcvaghy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/glwsmenyy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gtsyphopn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gzqnvtxeu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gmthqfwkc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gokhkbidh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/glcrhojok.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gscodtnnp.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/ggtxtmdzl.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gopitndbq.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gyxuxswci.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gcabmkyms.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gvmhrpkte.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gmdjlgfsx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gwtunwdzz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gamhgloxx.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/goaulebly.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gmxsfgiea.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gzgflhmqk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gzdjpifwt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gywremyzd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gkwxzfuet.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gftaklzzw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/ggiukpkne.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gyupqiept.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gyuyrsdrq.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/giauxeaxk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gondrteid.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gozocrtwj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/grjekrjjb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/goqdbcsav.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gicifsfjw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gvhjkgbua.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gjpssmbmu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gzgfyjocp.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/grckzhmpi.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gzatfmesv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/givyxpmlk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gbantpudw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/ghnzpmehw.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/ghmqxzjme.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gfmjcxzqm.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gopkdpbtl.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/ghvjpoyte.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gxujaexug.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gzjrgxoty.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gdcvzovlr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gftvlbylw.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/guqgvfozs.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gxomoyuay.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/guodcbhas.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gjckykrhk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnrrvrmle.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gweegofmu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gdvxwixqp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gdxnuafpt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gnpwdggao.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gwfgicygl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gmjonrlpl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gpvxwfwgc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gyhztgyzn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/grcehcxra.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gpxdwkosc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gkldqvihp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/grswltpmr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gdxliaayy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gpshbkaum.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gwsklafrw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gvuykguvc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gracsixht.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gsirrsrvo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsowedauz.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gxitxyzow.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsapivbpn.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gkjkjvsoa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gzzcxddcf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggugchsxj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gwepcekqe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gkjrripkh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/goscufxqm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/ghikbxtlc.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyoqqxkys.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbmwmogwp.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gydulbero.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gpveecrec.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gczmllmig.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gqgwroeid.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gjrizzfio.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gqnnqxinx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gnmnnydsf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gnypohmac.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gsbzngajl.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gqycamomb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gpqvaoaup.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gftrkxpdz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gvgygxalz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/glaemhzex.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gnjijmkvf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/glehcjhiu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gvwxiruav.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gxxjyhrrj.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gyjcwfyhp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gzfrrhqwq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gvfdqrrzh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gnkrhpktj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gdsnsrrvc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/guckrbprj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/ghptwdkoa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/grkejcpvm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gddwheasl.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gppyuewqe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gmugcffba.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfibsdvct.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gflsxvuyt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtfqlnsqh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gzrctoeof.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/ghdqwnjtf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grfnrnatr.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gocsgfylz.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gnkokepgr.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjmgemlmo.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdfnxbaat.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gafaaymkj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdqutmhvx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gpsjquovd.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxtzbuawr.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwtuwyhay.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxxpkcigj.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gifgaxdfn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gecqbgnkm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gevymipyc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gkjaupaaj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gsqdedlqr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gqcryvghz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/giveiglau.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/griiooahk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gjgamaxkm.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/glkqqxzda.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gujholjzl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gxfrltpyp.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gywzrbxex.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gmywcsxwy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/griqjlnty.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gfahellix.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/goqdytrfx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gauqkvcfw.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gxxtojzod.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkovyducj.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gpmiurznz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gupsbsiyw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/goypzutdw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gpvhfkifl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gbmigpvcf.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmdxsqsfb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/grfxzdras.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gefrqubwv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqsyayffa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/ggghbpgmy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqnccjuon.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grpgpeifb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gnusnycuh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxvtsailc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gchpaokgz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkgobnoam.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gjdmsqqou.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gaqahngvw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gpgrymrjz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gqneciiqi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gjwdewuam.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/goqdeizww.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gdoolsfes.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gldbqkgxg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gvziddqbc.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gpnjmdhmg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gnhaztevc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gwyljzlmr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gjcdahrvg.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gtoplilsi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gyvjnoxev.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gnrndghep.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gfloypeyz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gvufqlygq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxunxsemd.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gdebvkvel.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpzgcmehg.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gmatlrdly.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gcdfpdrog.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/glmiqnlva.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdxbfcuyq.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gdguphkol.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/giumjrbdp.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gyorhyjmd.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/grmqlkgnn.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gkyfdygej.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gsdazscpv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/ghmdanqjc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gatsemumt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gqogemvgi.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gpcxketry.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gwvcvblgu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gxkiawrmo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gdfbottaj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gtraeqson.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gmcyfelbl.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gufgrqqme.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gchzhonps.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gjetasnja.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gauhhshkt.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gvdrrfnxn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gabrvmjtp.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gjxjgkpts.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzqutddxp.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gucxhpdxa.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gzaieharj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gnqmvwjkr.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gcnvlpgln.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ggncseqtw.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gbpaygdsl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/guwmhclwt.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gefvkmarj.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/grwupwmzq.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gjqgsontf.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gdlheazeb.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gplwoyqhf.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/geokqflry.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gxarntckz.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gsexgjtnf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gmtakfsfs.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gzblndyvh.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gvayblpfe.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/glodhivov.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gbvyqsnxn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvzwwlkcc.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gihlsgcve.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gpddjhujx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gfedeqhyv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gzvkgkkhr.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/ggwjwfavk.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gxwjpooqk.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gainwptcz.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gnrnkhzjx.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gmxapvbma.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gpvmmngvb.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gjkgcbtcb.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gumlgpsgv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gtslxgcxg.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/goaquauxv.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gbqupjubv.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gzkgazxzq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/giudllkeq.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gkdzkkatf.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/guircmwjn.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gvpfrxxlh.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/ggmgolgoa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/ghrkuhtzi.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gcxktqfle.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gttxbqnwx.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/glkqiizca.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gdfijhjwm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gaztnqops.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/ginrnxrtx.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/grlrxjksx.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcwrkbrro.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gjyiexeqo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gaxuhiypk.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gxzqhxodx.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gzhmalxls.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gpuviedyo.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gbwjfmlgu.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gzamsheai.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gsxsxbpxe.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gkynnxlmz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/glpnzlnnc.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gcbjahcep.sHtML


<!-- 参考信息 -->