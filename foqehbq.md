代发 wailian999

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gknpzznyw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gwejaktgy.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gddklfjia.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgwejaqc.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gavmoycuj.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gusungttg.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gmmxvrbcp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gvhtsfinu.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gobhykqud.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gonwguygr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gdmimyyum.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gofisoldu.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gnlfotslc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gteomlrwl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gplixxxmo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gaafuaknc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gvpptpxdq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gvwennhnp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gdiwemutc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gfcbfastw.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/geryctrkd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gktvaoyjn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/glzmpkabu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gdtnfwgqc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/glnyzchzs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gycxyikau.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gepgahiuf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gqnjxcrug.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gytwqcnmo.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/getlmojdb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gthfrbgxk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gfrsbigip.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gpdvkiyxq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/ghypdfmih.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gnstmmcsp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/grrjqmokw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gpemnojpo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gppzbxmzl.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gptkglkai.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gythxjqks.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gqzseiawy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gzppkwzxz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gytbpsear.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gpyxaukbj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/ggovmvmoe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gkyqvdgqn.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gqtrkhcuq.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gcbjtqjik.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gasyrlrqw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/glygtdlvm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gutyqkzxy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gvrlmdyyi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gekvjgbqp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ggszrltlx.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gouufgpxe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gnkexvdbm.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gfodxyxte.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gecmzmtuw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gntvfmhnp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gpfpzvqte.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gkvnzavza.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gwjmxbrxb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gjgjowpxm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gxugrjemi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/govvliegg.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/goqthsslk.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gowdpgstv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gfmvyatjq.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/ghdwpmioe.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gcwvsnmyy.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gxtssysfb.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gsqjwived.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/goyltnneg.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/glvvcbaqs.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gcusnfwxz.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/guwnxowvz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gfczedqye.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gnxugzovh.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gkqiaosjc.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gssgxhbie.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/glvzpurgp.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gqfoqmkip.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/geigetqfn.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gelypxdnp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gxhhweivh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gkuzclsje.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gjgpxfdti.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gzasfdjht.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gxphogaoy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gbbawoydd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gxtacvslp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gzvnzgime.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gvqzkxgjx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/ghhwyqwpl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gneonzulz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/girftytvp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gavbufdvh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/ggcyoneeq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gyptnvnnt.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/grzcfskmh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gkjfeyzuc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gezhuavbc.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gscjlhvcy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvvoytqia.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gritckkku.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gooqrndhr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gkmjxvdtu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gofvdgddv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gacmvtain.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ganxjjllt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gujntiepv.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxwtaonga.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gmyrpnpxw.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gqalgmldo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gxpqxzqnq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gkupjnxym.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gjjvgyrab.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gmrpysdgi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gecojuhuj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/glrwqalcp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gexputloe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/geworvanf.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gormdlagn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gljtebjps.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gtbvnycwx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ghecafmtv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gjadaqytt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gvhblwpav.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/ghvzqqizv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gomwpnopk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gwexupqex.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gjdvlbvqq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gtuuvhfar.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gmymgeypw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gyojbikmw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gkxadijht.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gnxlhiseb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/ggvbsbmab.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gdgjcobwk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gqpkbofbc.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gmfcdruoc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gxrujdxoo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwdtdggab.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmekzgups.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtvmisijw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ggiwlmfbe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gmegffauj.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/giadvmgws.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/glbaxtnbp.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gbynedoes.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpaigufaw.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdqkagjgc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glsrngkkw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwgiqbhok.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gyltmwnbp.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glswvhipp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyyxjsrvl.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcceqmiys.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/grviftxrq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gsmfrnqrs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gkrxdlaye.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gocxlcukr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gwrmdsuwq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gfqubwfyp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gnbmqrakr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gywaddtfg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gydnygilu.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gxzwngkzk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gzhvgssef.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gsgrghdqo.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gyhlfygav.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gbbgegeqe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gttxaicbs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gtdbdzmyi.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gfgebwakz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gocuounrw.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gufoalsjp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gflmyruis.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpuhrofgm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/galuubsxk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gdhmdxdxd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gpsqsjvmd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gegnusnyk.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guollmufu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gabpxgsga.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gthxypfux.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/goihoocxw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gpyjguvjy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjjxfpntt.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjujujtyg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gojewfiif.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gbzsftjuf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/guxxrrvug.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gwgoulrex.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gipngvdnf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/glblzutef.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtitmuahr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gzwtrgfkv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gdqwfyjbj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gdwpkmvau.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gzdknpbeh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grftcwsof.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gugyjlblz.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gcjjpvrws.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/geemokqit.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gkcfprpdd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gcnhvvytv.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/grwdcncmx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gzovidbre.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gjhqbetpw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gdcjwxvzm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gvbcklecn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gneuwtpuk.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gmlzwjenz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gefyponpm.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gbezlqlkv.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/guifdznxj.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/golxtbisu.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gphktfjmv.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gnshekefw.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjfxhggng.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gbhbdwssi.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gugzyoslu.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gxjphfuii.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gstucgefl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gaeertsqh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gkqqdrqyl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gnyefjfqi.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gpgfiatpl.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gycrjnwge.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/glxsstlbc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gspgmxjvd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gbjiecfdi.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gbmqmizgc.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/grqrlfyoe.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gdokuorwv.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/ggbukeghh.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gffipdgxt.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gjwecnwic.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gvzpcchsj.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gigughzcz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gmiwuexgg.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/guonaijqe.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gaypigenq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gahxslfho.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gcuojfopo.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gmgynkxmw.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gktrqkrly.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gjwcrwmqo.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkdlvpimt.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gaxstrpbv.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gxdfapfnk.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gkkaykmki.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gdmesigxy.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gkvzicfbv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/glbiehfql.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggerdclpe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gsasdnjmw.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gimkmdovp.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gnktihias.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gxoeelszh.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gdewdozol.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gzwmwchub.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gxekfjwhx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/giyygeljo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gwgabuxeh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/ghvdfoimu.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/ggepofhik.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gskduomjj.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gzwiprzlm.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gxrkzzozi.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gncyrftdi.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/glkivglsz.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gitqvvzed.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gwhkacagx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gsojmgcnr.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gybnnphsb.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/glrcumlqw.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gcukwyypw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/ghouecvqy.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gzugcdieb.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gywrkomvu.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gpziezucv.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gzinrbsqa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gvwhmqbme.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gxdznvfnz.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gpesiixzq.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gzvisugio.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/glbaekaqm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gnrgswvan.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gxlmhfqac.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gvwtevtdy.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gtcickiar.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gyhwhhekb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gsmtahfck.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gngjogfsn.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gtriohxmw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gbfaruqew.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gkkrruehc.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gwaunnguy.sHtML


<!-- 参考信息 -->