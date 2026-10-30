代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/giqtzpadc.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gtsdwtgfr.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gogokeocn.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gbznshozt.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/ghzfclkyo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gluthofrv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gfejykqmx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gydkxqbad.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/geqgilxcn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gppblzzid.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gcgkfayky.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gngquxjkj.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gnskpexpq.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gkxzwmhwr.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gtksukiek.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gfbhsdkmh.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gltbrvein.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gcbhyeetd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/giuxzwaud.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gfjeecuyb.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gvfyqgihu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/grsfmodcz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gvnhrmkhk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gdownynfc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gtxitixsl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/guqptvsyd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/ggjsmqjvn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gudsbvmqs.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gibwdfjjc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gpggbahen.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gbxsvkxnf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gngvddchx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gpcaeqjqe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/ggomkubqy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gqsdeuycw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gpyvjyzpf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gaxssnblh.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/grrcpglcy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gafnelbgx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gvcwhrdrs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gjqslxjif.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gtfudjddd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gyjdjbezf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gcgzwvora.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gzblpvgil.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gttecpeio.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/ghnvlpwwe.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gkvthlura.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gehuwjzjc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gpbpjrjyt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gsjihdiso.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmlpucbx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gightpmdw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gvxtefrfz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gynhylccu.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/ghbmfvepd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gyhxoosoz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gkmqddbve.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gisyahgbs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gwmmzodms.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gpljdhxtr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gxrmjnamf.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gucbnmlhb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gqcuravpv.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gegxswdwq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gfdjetzez.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gzzzpkcgq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/grttiypjq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gmqguzjok.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/geyceqpau.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gzkoemygh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/ggngphywc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gcoqhonrz.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gpscbwyaw.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gpnkeezmi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/grbqckgob.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gqoamyuon.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gfgrieuxg.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gcqgdkecm.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gscixrezj.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gcnmjzjft.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/ggrkpqouv.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gwoyfmfwt.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gdaubejvr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gmersydcb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnsamjrje.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gvgzzdbik.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/geaobdeoq.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/ghhynzfzz.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gqoerrdbr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gyigxbtwq.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/guxnbzwqh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gngvhqlfa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/grdqhdnjr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gxrazduxu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/goofirdda.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gnejzuuwm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gqqteqwlt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gipdmzcnp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gfwqfuzel.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gohabpbbn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gysmewvte.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gwijikkyp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gucbdpfhv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/geoispnts.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/goykfemhr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gllqagtxr.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/glsyzoodb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gjbhrroul.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfphxgdpp.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gqualztuy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guwtxxcwy.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gexivfbmo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/grrrmvhmc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gvwfmoxiy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gaetvznje.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gqkdoepgs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gvhizwiiw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gfuldkrpz.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbbtiixhn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gagoaybnr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/giupfgegg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gtfcvukli.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gutkcutoi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gtwlyycfb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gnonzzfov.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/ghrpondrc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gwugfqrmx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gflhchifs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gpelanmnw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gsrjqszhh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/ghaycywkm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gzilhgklw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gxrmxwwli.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gwnbbzyxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gturkhxiz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gtusnmzsr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/goqswkygh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gjiocbdef.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/ghjcarayi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gvfyjigdm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gzlpcaryj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gvrtmqyvi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/goytobjux.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gexbvhaha.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gjfueznqj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gmklrrtwb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gdlivqtbt.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gcinmqtdm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gvhovkdoq.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gnyqvhifi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmsjkwgtm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmmhnyptg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gofcunksy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gstlndnxx.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqoydlkav.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdaowzjxe.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gkqjpjbom.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/graepmbin.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/glqdhvaht.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfiabogja.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gclinwxjn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/galisrsmr.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gydhgwxaz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvlifglyk.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gudzkrxvw.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gajwdxflk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gyfyinaaj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gxrfqixay.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gichulwbs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/grrrbzsyl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/ghveneysn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gdvvfipcx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gdvtnsrdc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gkcffeoof.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gxjvugpox.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gyguhusih.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gsjcuuhdh.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gizfdvihl.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gdptvqglk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gplpqubcf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gfkvvfkhn.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gssidhcys.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gyylxiduc.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gtymhymfb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyrdkmfdg.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbuowimqq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gfbhawuuf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/grufatmme.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gntfxeovh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gtdoiesmd.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gphmguefx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gtyqulxfu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/giaztdazk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvbqjjbfn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsegwybjn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gryvbuzdn.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvfkmbrcc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/geirmferq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqafxruht.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gewsvqens.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/giqpbntsw.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gwbqjpsdl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gilhgormd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gglaudetu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gcsegjrds.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvjfpjsry.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ggetihvaj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/grczhsqdi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gtygpegoi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gxkfofajb.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/geqtbqffr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gypxfdlzy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gplhvekad.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gwqlabfmx.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gsmpmndha.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gtoicfjxv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gokvqupao.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/grraoxfyc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gczvdwvpg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfllfqlti.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gttiedkft.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gasesurey.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/glgnftyre.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gwopnzktk.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gvhnfrrhk.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gprtxuaqa.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gkwmhtjru.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggloiqsck.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gbbgupaax.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gmzacgmix.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gwkgyrlgj.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gfenmaryq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gwmwegssp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gjhnqllkd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/ggruafezl.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gmaqmyksy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gydvvdrvs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gwydalzdi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gsxrjqeuo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gjeckeqow.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/goymtktzy.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gbwwxfxvp.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gadnavbjo.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gsaylhpft.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gcjngxadk.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gwdwntugr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gcbykaxuh.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gqmdntgti.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gexjoegay.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gojhkgiwv.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gmgbpzzap.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gueknutve.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gepolgqme.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gglfzsdmm.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gwmceivxp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gvrkpgxxs.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gapzfnwul.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gjawwamxj.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gmdojplak.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gluxekenv.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gimhlyiad.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/goqfhekec.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gvvjgzbwv.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gxyezrurp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gkbwkpkjk.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gpbntzbyr.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gwhiwiucq.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gzpeewywu.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/ghilmgpfr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gshhoxcnx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gfskduyzg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gajsfoppc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/goofvillh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gggtbswdi.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gvlltxwcu.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gwpemyzzi.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/goygdwnxw.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/guklhdarr.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/geykrvpnk.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gqjvipunh.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gsvdewgdq.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gwchasgus.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/ggwsqukbp.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gugamtybd.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gpbwskfgn.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gqqsugtrw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gytnmkufd.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gddfxjinl.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gttcuqxpd.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gxfuazhib.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gnakqdfwj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gasimoqee.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gfskzorlj.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxsbodydx.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/guakejgmw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gwgsslvev.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gvrhlefwm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gdwkmoyjc.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gahijrkwq.sHtML


<!-- 参考信息 -->