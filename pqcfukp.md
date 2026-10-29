代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/guepkcoyq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gtvqepqob.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gmwiwawaa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/ginrzifzs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gsrovolev.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/groinvmez.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gmyqzjgip.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gynrhgxjg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gimzfxfsu.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gkokbicbd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gbaqemshz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/goiboelbn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gzdxzmowe.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gobcptxrm.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/ggflfhvyb.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gbxmxzsam.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/grcnkzknt.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gzgfoxayu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gdsnwapvx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/giiebvdln.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gkbhkoxlk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gsyiixbuh.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gtozsflqn.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/grjwczzft.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gjrfzkuvh.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gtyyvgkdl.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gfllhpqjj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gdadrqbju.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gopssusii.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gbdyuamjv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gwajuzoja.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/ghudjfjmk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gaqxqqlam.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxvqjodn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gpxqqfovv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gfgniryox.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gzuwvgmfm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gvthumbvv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gaykyjcsf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gfbyplkqu.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gtompsvrg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gfrdiwzrp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gewbotpde.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gfdxjunru.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqbmrmta.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gvjfrzeqp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/grzgimvec.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gmjpapith.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gfikhegbr.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gjkueqqxe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gkpybhbsi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gtbcsavhd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/grrrhehxa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/ggosucomw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gpxavdkkj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gwvkdewpp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gdsqmmdok.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/grlpksfvs.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gmqohjzrt.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gryiqwemv.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gzxjewvas.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gcstpvolz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gohjlfgpi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/geofuzpcm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gnmujrori.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gfgknyalc.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gzvipjnsx.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gmzpcvsgf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gltafhzel.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gfcnemnfz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gqcizcuks.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gsveqkrxp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gtoihemvx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gyzjzymjd.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gxoeyboyp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/ghlzhrjwg.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gwklmwdov.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gkdnqkbuo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gtkekbplf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/grgbtxous.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/geygxgsxy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/guhglcemy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gsmvvgxem.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gbtxohrje.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gzjlewfxq.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gpmplvlvr.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gubvoibuz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gbbposljr.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gvhavgtkc.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gobfjdzsd.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gdobyjlit.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gpihfhbgt.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gpmtpfeur.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/ggqjcvugp.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gfmbqxirn.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gxvandgnq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/giycdjbtg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gdledfzwl.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gfhfalbmx.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gmlkaebjg.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gndlbmgcj.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gcjwwpmfv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/guxbjcvyo.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gptdkpkbd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gxkutjzsp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gubvkkevq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gnnwgaemt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvmljenbx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gptueubqd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gthwuwmsq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gygzghvyr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/ggkxndxyo.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gmuhjuumo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gbxzwnqsa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gbkfoksrb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gyiurjopz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gtzmmkhsi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gqahbcuzl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gvmsckicr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/glufojenj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gtnumuiwm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcuuutlad.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gjjsabjcz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyfketujc.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gttibycrp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gxtpjbfny.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwbacpvvk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gcijamvox.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gdnnwaszr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gxdtcnwyd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gpaqywxfp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gydfkooro.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/girobxesq.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gmiuotxas.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/glalfvasl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gdsfblhto.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gjiuakpxo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggfswenpq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/grnwnhmmk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gcislukez.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gtuannjrx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/geeznytxc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gpwbxoqxq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gozhwgqjl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gjpqwqrlg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gccwqfxkf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gklyohghx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gdwezkqtl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gsgigihvz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gkzvupdsi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/guesyqkvc.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gmljpirft.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gqwimzavj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gxjhvnlrx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/glfinxfxu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gitvkisls.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/ggopmnadm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gugcpnnow.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gofofcsgt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gysrzlmyj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gpgbhnwtk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gjiqbkudf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gegittsjl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzkveqgpi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gigfixfov.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ggjfgmumh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gfzxlxktn.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghxmacsrn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gombgtcwj.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gjwhqmikx.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gishutqdl.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjlncxnnm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gatgasgfj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwqcyhbox.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gqhjoatks.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkttqnssa.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmkjdyewe.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gayiqhink.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gadxzrswz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gyliybotd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gbhqnzoed.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gkpdfuwsl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gpjitcdtl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gzwcdsauc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gghzapprj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gtmcxfmyv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gnvhaparf.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/goxhntzbn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gxllzmqck.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gfgxoxtxp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gekzjcmas.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gfnupyssi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/griccbuhd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gsnjtkock.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gwctwrfdj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gybqonesr.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gabdljdes.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdxnjgzmb.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmtstiiit.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gzkaryudf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gnpeufppc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gjckodzlv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gbkkrrtje.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxyuoxwos.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gimaaqvix.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/geqsucyam.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gopiqmxms.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gxrbxacvc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ggjkrwmmc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxqcidnjz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gzfaajwzn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkytsvlnc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/giqarpixa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdhbezolx.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gsklxqqvf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/goffgsmlg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/glskfvtuf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gwxkteqci.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gracodvru.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gerxfrllr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gtmmoyvnu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gfxfqiwrl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gyyhtauid.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gueolcctw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/goiyvlsqw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gooxdangc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/grikyngfm.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gkrrbjajb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gusmadrvr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/grmcmrlll.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gmdfooaic.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gskozhglr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giedfipxo.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/ghwdlqsfh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpewluiun.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/ggzdmzawt.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gpvraaeas.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gamibtatd.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gibljyjrm.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/ghismpbqn.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gbcpekzbf.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gvznjskup.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/ghocmoeyw.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gosakbgia.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/glysgnape.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gtzjpstty.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/ggyfpvvdr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gyehmbdli.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gccypurrt.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gcmavkeky.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gyheszlxr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gdsxtjnny.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gtztemten.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gtyhfzdtc.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/glkhpukvf.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gbiqhrmoc.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gdsompmfe.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gigjjvoip.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gdsqcozui.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gyvgqffsx.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gxxyaxtuc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/goovkkoso.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gynogwrln.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gaglmbmxy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gnmyxrnhr.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gfggiqhmk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ghhhavony.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gdvtzauxo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gqutpjqrb.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gcahdivzv.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gsozpdavl.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gfyzduobd.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/grzopeflh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gcecpkvlo.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbozedhbh.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/giiyhyogg.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/govmelayi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/ggytlbogm.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gsvijmsld.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gawfajhtu.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gxhqxeffp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gtsqsopml.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gieecbqad.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gomqgquqf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gppecomrq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvajkygtt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gsfrzqpqj.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gytjoevjs.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gzpudvhyp.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gtjzgpjdp.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gfdqapcab.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gpkmnrwqh.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gbwmxnnmi.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gpridgmmd.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/guwpspvfc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/grntypfoi.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gqrdnjuzh.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gxxvvzrjw.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/guwnirndm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gofenmbbp.sHtML


<!-- 参考信息 -->