代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gzjaweaqr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/grrupjhve.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gjalcpzag.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gahkvzlua.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gmnjiwxqy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gcxzxmlgg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gtzkiwixm.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gtrnnzoar.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ggwbbcqjt.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gqojmgrjb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/guikyjwzg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gwlhqerxw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/glymhdumq.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkaacdblt.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gruiztqwc.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gtugnpegp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gnpfexlzm.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gryxolufc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gorzzormt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gihdmsekq.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gdqblfdvd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gtorhylwt.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gmoibfiwj.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/guzpqxmmk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gtvwfhyhk.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gnviatngx.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gfrviotsl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gfmzwbtxz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gsnmzxmwg.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/ggdqeiwec.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gpooxodmq.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gadgpiksm.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/ggnwnmyvw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gxilqjqwk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gpigcfzrp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gdupgqrtz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gmbbuzjvg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gcolhfnhk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gnptufaei.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gmusjlbsx.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/goyhlokaz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/ghpxklufk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gxyoqsxpp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gbxdqscyu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gbygiarex.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gfgwngyyc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gtlumcmxs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gtelqrcxl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gkbfdhdfr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gfbpzimrp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gjtvxbigr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gynnrvill.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gtbrvrjdd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gwhnzmzlo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gdqshngby.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gioknwrrg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gjogokpbr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gmavapfiu.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gfhbaldln.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gqiviwppa.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/grsudchjj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gcxpzefdy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gdnnrcpnu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gxweitdro.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gfotfxnzk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gurhkgrvf.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gtsmoqwvh.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gfvcxuazm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gkuaedhyb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpcgcttri.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gtcjmqvux.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gpsejuwzm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gojkblmwg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/govllwpzw.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gjqpwuwmw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gsqbylbaz.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gccoyptrk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/grnmnwclr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/goycpbuqx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gftrsvnee.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gjfhltvxi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gefsrmhat.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gclhdpfbm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gphipzdiu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gpmhedfdo.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gjjurhzbg.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gwuvqjeyq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gyjqwumhm.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/glmaxhhtr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gkfvnblsq.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gzohfljtj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gpcrsjrse.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gaanahqpf.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gjqdckbyo.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gkklhaqei.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gosmvtolz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gffcttnoc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gglfnsgrm.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gznfscwyr.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gnwfjbgvk.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gxejbizss.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gijgbklhv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gahrlwsvx.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gcjmozocb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gwmnewtim.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gcknzbjyy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gkzxanyiy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/goyemtfwc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gahiwzxnj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gykffsvdc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/grlmydtrg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gidvnliyj.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gpuqlynwb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gyqxdrtox.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gpmexugzv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ghbawgtuu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/grrpvepvj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gtphpxjtv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/grxvxmbsv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwlehthcc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/geivpiwgs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaucmzzrb.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gpddpivbc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnetfyisg.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gwedllfcy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/glwhwtsoi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/glxzppquw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/grjxkoapu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gghhqlohi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gbakicgli.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/grfzlfvew.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzvilretz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtabznpfe.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gtuexeazo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gdqfovbmd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gnmnsnqfx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsmnllzst.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gzamdpdmw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gbobjhxea.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gqukkzjcj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/ghwfbzbzt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gturtkgam.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/glftutquj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gbjgpvotp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gfgqpkxmx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gietejpdc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/giykoxxoz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/grqnlbpea.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gkdtfkvog.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gnrylibom.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gqevakyrm.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gfpbygfhr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gtxgrzsyc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gdzcbcfus.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gqmjfclda.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gkaoveely.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gvjcrcozp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gzuigtuzk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gqiozbrtk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/giibnbpkd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gfjjroovq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gxogaazch.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gokjrmocu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gievhaoqe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gduytgdat.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gqrmfebcw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gesgpdklz.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glloxfukg.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvxvrvqcl.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gtyyumptc.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gaqujqena.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gguldyaxu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkhmxaqmp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfpfsfiug.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/guudegrzr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gossigbue.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvpgthvae.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/goajdqkxa.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gpdteqnbe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gwpdiijtm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gvxobxpar.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gdoigjitv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gdmmgkjpd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gdgfjxeoe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gwbsatuqr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gnusfasst.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gvjynqaou.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gqqeyjtgr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gejylihua.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gqqrpaxng.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gdwzchmnn.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gwgoojqck.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gaedfumvi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gnkfqplqb.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gsusqkrbg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/glidoyjhu.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/ggnywvgeu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpuqxoylr.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmqlfjhwv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gbrnzgyzy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gyqnyquyz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/guqqjzndf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gtldgswlh.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/graselrvh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/geglcnigy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gpzvpqzjg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/glcftjztv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gdfkmytpt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpylcleho.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gorsiqhot.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/ghkrhyrgg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdrmiqwyw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gxedgtptd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gicpdldjl.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/glgxjjhaf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gpylcoskd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggqnidxnm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gfbfryprv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpzigdool.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gycqrhhja.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gvbteidcz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjwfrhjjk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gvsdsazdy.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gwafcljfy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gdgqlbxbm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gzucuoqqc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gfuzkrjkw.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gxhqryifg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gjaadsnno.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gdlqwjdcf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gsfrfczxr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gkihzwxaz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwylrvqyh.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gobjxdckw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqsazzpcg.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gplzjhyal.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gigltooxc.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gdjekahey.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/guyvupcbl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gdzurtapf.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gdhaaxdod.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gwgvfjofe.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gahcvtlfr.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gwssujkjx.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/ghsubclsf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gmtanwsah.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gjmijkxyn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gpiufoawe.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/goimendsr.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gnfhbsssq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtfffogx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gnzkpntwl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/grrbqdtxd.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gbzeprcoo.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gtgbnvrea.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gihrstgce.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gowxegycf.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/ggvobatpq.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gxdksxsom.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gmocppirf.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gtwfrrydj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gpwwjpwsr.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gtskqmhqt.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gsqdaevgk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gpkymgskg.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gjudagjwk.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gdmuojsyq.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gubpkmbfj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/grajzvzbo.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/grhqyvlam.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gvbnspmvh.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gtwtgqbju.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/ghhtizohx.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gdgxmljhm.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/guommkqwt.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/glqvdkhfi.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gogrgcxwq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gdmoghdeq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gbezdmcaj.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gdqxkggiv.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gzwijojll.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gfokjmkyx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gekgbibuw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gjkdlaqgc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gecqybnri.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gyuutrhvg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gufoxzcvw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gsmjgbzbf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/ggkimrrla.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/guexsunwv.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gdixbrlfx.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/ggpbgmlab.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gflkfepgn.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gmezqqfqv.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gdeevqxvb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gjsjmpfjn.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gjyifisod.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/garzdsudl.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/ghxgexheh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gnkwocwlr.sHtML


<!-- 参考信息 -->