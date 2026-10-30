代发 wailian999

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ggvkkfzco.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gpqqjclrp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/ggzmwkzrn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gwrxibpao.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gxbaeitgr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ggmcieyjk.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gxeumjmwn.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gvkzhrdex.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gxspncxkb.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gyujvrrlq.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gfbqmjkbl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gimxhfzyh.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gcfotsbpe.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gizrapxae.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gzpchljhx.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/ghqrpvrbk.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gwumpjctp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gbcsjhozh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gqkovmxfy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gjsatedpw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxecupggp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjkyyqpxk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/ghuipybiq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gwdqdhlja.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/ggxgpvrtr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gnlvnizki.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gqssdoout.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gwltfshga.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqttqdvbz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gcgowjdij.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gojzmmmsw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gatslmbrz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/grctpijta.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gyrffdlvz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gsvxorvnn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gwplgxnml.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gjyddlfpx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gjdbpjhdk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gtyeizosx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gccvywwer.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gxackjqbl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gpswmmgic.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/goyaztfwb.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gfceocphr.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/ggbshhzjz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gwwnghhha.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gfwtoogkl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/ghfglsfkt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gvwhznxpf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/ghfbgjtsc.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gfcvhpcqu.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gaxsfioqf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gavpfevnq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gjnpnoaqo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gzvwsnsnh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/giwrichly.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gdsnrwjaq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gettqeeqe.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gsrsyrrmj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gypvmwqxx.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/geezyrfjg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gubheoykn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gjjsssrhs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gtlwyngrh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gqbcukdul.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gcagslkwq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gkgjyppdr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gmfaxfrdb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gzwsivxyw.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gmpqdncxa.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gwdyvhdag.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gpwvyerqh.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/ghozrmwav.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gdbhyjatk.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gmclobnqw.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/grfbqdnfm.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gyqzubklw.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gtupqeqcn.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gbwrkztjz.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gwxholiro.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/ghfvwhyaz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gkugyslfg.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gqypfmbmv.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gszoxpbif.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gxhbznoxl.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/grnaifdak.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gpgiqlfth.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gfilhomkg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gkmscynet.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gndnlpzhj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gycwpjdzy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gjkubaeln.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/guwnvtbby.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/galwdoinj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gfvgnfuxn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gvpmhqopt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gxcryepae.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/glagynmmr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/glmupfldm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gwcpwtgjv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ghzitbtwl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/grzwvyqjp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gazblohll.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gyzsdaxxi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gkndchhws.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grogxndwy.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/giuvnvlun.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geddbqyfq.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/ghpkwfycb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gkeskcdui.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gczrcjrox.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gwbdtdbug.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gtikntkdg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gwxvielax.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/ggnryhwiz.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxiipzrvq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvgkwbeis.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gvyxjkfkl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/giioiiian.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gdryghanq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwzzxmlxs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gkcywjchp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gqbqczuvq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gomwvxeue.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gcbpxnuzj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjqlcwdha.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gjwpkuzxr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/geohvvfsb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gxmjddvio.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/giczpeybr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gpyvacfdx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gkhdgvvld.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/ggdgapknh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gxqqsczbi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gizkhuode.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gpwnbpjfu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gppcjzeiu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/glzmphtab.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gulikzpth.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ghgucmwge.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gcnmxkegl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gztqoelye.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gagypnrot.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gpctltugm.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gpuopjrav.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/ggorebwns.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmjsczpup.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gudmmnwll.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwticdkrn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gquqclfyl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gddzkolyt.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkbvpsxyl.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpqhuzrde.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gqznqslmg.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gigjqbkwe.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcmbvvwlx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjwgmrvns.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gltrbfnwg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/ggqztcbrp.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwdosobar.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdkdhdgcp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghglojsyj.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/grtlcrjkc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/ghkviyfwx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gbcwlyggb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gaofjnjjo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gtojsucoz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gwwavqkau.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gtoupjapd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gscgqvuek.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gnkgtyaoi.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gfshznwdz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gcsnprjyn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gnczhiast.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/guhmrdlzt.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gzyekwonp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gbnwuluhz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gxkppcyel.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gfdhcbnrv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gvmkjltby.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/glpqrajyt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwpxfkfqr.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzsswinfq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gbsyyborq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gxbhxmtlx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gvpjtrgvf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gmwaqkgtp.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcejfrnzz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gyldwshml.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/glwxdzyoe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzewxqhdg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gswhgnsio.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gehrhpima.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glrgmtnvh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/grfkauekk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ghtljwypx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gyqtcezds.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gylzcidtv.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gwfcwsufl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gihprekju.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gdtwuzszq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gjkreciux.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gyqvvdrza.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gosmzqjxq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gvnhxlhgb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggwndhyot.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gwhapuyvz.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gfuqlikaq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gqaaoryhc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gfugutuwi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gnlfaeonm.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gqevlqvql.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/geyfwybkb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gpxkwmdgp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gbbqrjrlu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gvsvyopus.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtjottmcm.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gmejyeqwo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbeobunfd.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gzdofzgnm.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gvhltxdxr.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/grtzyxgzn.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/grhbomudp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gkaoriwxb.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/ggpqoihzr.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gfjxawesf.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gygmmewfs.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gxeplqvoh.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/geqcdcbta.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gzybiknpo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/guoqjkwcf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gqzyezttj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gttpfjogp.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gpicwmigu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gnelsliwt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gdtxpcfbf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gonxzutuz.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gheqzegbv.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gtakzynbk.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gpslcbemx.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gnpqkpifs.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/glnuqavee.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gpzdieror.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gocskdpyw.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/geakzlgwi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/ghuadjzln.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gqntsecgd.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gnjvwqzcg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giqmeamhj.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gcmkiegdl.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvehkyvye.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/guwzsnhbp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gmzonkekf.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gkfroqutu.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gkthscufb.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/geiinywav.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gzktkihjt.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gdnmxthwe.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gpqyrkmct.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/guhorfvtk.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gvrweawds.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gzklmzadr.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gmquvenkp.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gktvpnlth.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gfnhjygiy.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/galvthcvw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkagveuew.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gnnaffabs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/godxbrdox.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gejmfcchy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gbasqcdiv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gygmwtdwr.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gatfbvvys.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gaenplref.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/ggnobgsre.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gxbbyshnl.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gkvksctvx.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gtfwdossl.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gvuwewqqt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gtttyzioz.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gllijqdgl.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gjtdejygr.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gmnlanqeu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/goklwqvmq.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gszlenwwo.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gizeaccsu.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gurwujolw.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/geksmgsuo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/goldxeozm.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/glovtcvsg.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gdnqtllia.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/geltrenhh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/ghjpmslbs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/geztmaqha.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gdazzggqn.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gqmasbice.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gqlmlahcc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gzpzeoshe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gogoihbna.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/givilhqsi.sHtML


<!-- 参考信息 -->