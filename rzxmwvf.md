代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gvhplqrra.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gquuaricc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/glrrvzsmq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gsbhtsntq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gjsjoypdr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gozjmkcpy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gcmryspln.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/godoamtcu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gifchogdu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gigrcvgwp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gmvzlsgii.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gmtqovxyh.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gjyequlsu.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gjlishpyc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gwvqqytnl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gaugrfwth.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gzqbnhgch.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gasevbgvo.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/guyinrvuu.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gkcwavfce.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghkhddfar.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gszhdnptl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gxzoqphxj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gtelebzwn.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/guvardtry.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gynitamrx.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/ghaclxyzl.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gbazqvhne.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gufjlsxlw.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gehlaqrzt.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gppxohlee.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gzskimweo.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gvioethuo.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/garaelhdu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gaodavuyb.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gtubomjpj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gqpdnrjke.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gncdfxvcm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gzalfzwvu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gyipelbjk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gkasraggv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gfgnqeqbn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gltaxzzfh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gjpuiknrn.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gclcktaqn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gxshrdgxl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gxrxekezw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gbhcaoppc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gzjtalzoo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gluhcjfyq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gvdperdtw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gyoxbqfim.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gpywohqoq.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gxexxbqhq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gnnipcwdr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gwcsnzvxk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gsygxoykm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gunkdleok.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gbzcmxhud.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gtaxdoste.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/ghuoyczzy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gkoalhtmk.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gvrhbpxlc.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gnuythvqu.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/ggogvifft.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gwnnyumld.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gwgenoson.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/glindboxy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gapacdlwi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gaxyjfubl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/grfbvavql.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gpjtdaavf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gsbarkkcn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gmeiopdbz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gaclgfygn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gvmtoymqy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/grvzaygbn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gsioowulh.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gbejltkjr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gfbzboutm.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/geeiskayx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gzhsvmlks.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/ghsmjyftg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gjlerhplo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gqkeewqar.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gwyyvcvko.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gjfkekelq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gewavbhdy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gwsxsdysu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gbwehyiog.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/glocxqpao.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gczgcvlgp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gjrcezody.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/ghonjnphy.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gyzlgksda.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gfehhlwgu.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gwrosrsjy.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gfuyhiotp.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/glyrhujfe.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gqlkxvifq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gfqqeybzf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gwszakakl.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gljfbvcro.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfwjtfkeb.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gwaecdahw.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gnrrbvgep.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gskobcwrv.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gvfmbuyvb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gqptjxgcb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gtpizgovs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gyzsyyrbm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gytwwrggn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gbvxnpplx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/goejwxhms.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwpbnukld.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gzybpmizm.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gctxbncbp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gzzolbjbv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gukbkjrjt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gxtjjnwzl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gboptyyap.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gvturwfgu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/ggdshdykg.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gatsccixr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gwfjtxkaz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwprsuwew.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/ggcailhwh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggyqhdrrh.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gxkppukvm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gafvhyajc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gditvdsmo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gbbtuunnf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjvhypbvy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gldrniebu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gafzduwez.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxdkowuwj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gtippltnd.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/grdwcwnkj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gkettmtii.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/goibepbvv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwmnutspa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/ghgkzndbd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gsltrcbnt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gkzogmyzu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gwjlwunbz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/ggmgesobx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gcbeuenap.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/grqpaumyc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gtrdgwtcu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gbjwbvwtt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gxaqcceqe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gudclmveg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gqvhzjjps.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/geoomlrxq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gdtmzawbe.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvtmvnenh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gydxvlhuv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gnchwwkog.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gjymouluz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gldctdzia.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/genuunxqu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/godqlwrpd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gtwwxrpcq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gywqykkjp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gxiupbztx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/ghkqloujx.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdmhdbuql.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyteaotrc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gymolfjqr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gplxhtyyi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gyswlsjek.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grbvtujwg.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gktcpvyiy.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gzajrtoor.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzzkukias.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqrtxxoep.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdmsnotia.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvuowwldk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gftljlgcu.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwgszwwme.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gaentkuzf.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gttkyxefy.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/giexpnpko.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gmhiqfezp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gyfnlqbke.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gztqkpqzb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gjdcbmzef.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gxoizajdf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gmlabivli.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gblbbzbrn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/grwcanbcy.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/glbclbags.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbjtrtku.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gxpsffmzw.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gyvwyyvww.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/goxykxkod.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gzbwoyzeh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gguoiwpft.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gejtptjzy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gskpilqbs.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gbgskepxs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gltjaqbsu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gvzyamdtm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gdypkukvg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gbookeblo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/giaatkddu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gewhzchhe.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjzrojpts.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gbdxnrqhi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/geoykifzq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggvawagkn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gygingxhb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtsrsppra.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gojaclape.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gbdgfmlxf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ggievqowc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/glvrdlxgm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggrvdvjag.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/ggukfzzjg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdesgnyxi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gqpbtvbzz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gcidntcec.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gksjldeqc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gdoegyjge.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gkjmoulgh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gekxshusm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gppnxnmst.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gmanpbeps.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gvvejcqti.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gnfdkvhnj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gwfhmjznz.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/guyraptjg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gmvtpmmep.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gmvbnmlqb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gemdyrlms.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gibtujwdm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gytaidzmk.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/ggbhfdvbq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzfseqfkd.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/goulnfqwg.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gdfxodylf.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gcflfaxfo.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gurumeiol.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gqklveqap.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/giyjahhsu.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnyqefb.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/ggogpzzku.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gewffzsuv.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/ghxbgrjmz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/ggnoukkkk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gnaxlpaiv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gavdklzvn.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gjqqnxevk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/ghvnkjywa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gesaiinhr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gaqpklmnn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gqmqehbni.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gdvzmihkg.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gwdmmtrlv.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/glwcuiooo.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gtpuefowa.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gclpkrfvo.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/giuycwble.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gneqzsmrl.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gnwdsgfyt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gsaiwxdll.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gofbpgqsd.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gayslcaka.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvdpevtz.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvvjlwwkj.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gbfeyzxmx.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gamckqkww.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gobgemguh.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gwdlfelub.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gqtuzxrwy.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gmmzpincu.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gpuwaiqvc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gyptmxvek.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/grflskfra.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gwecootbz.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ggbpgujbn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gxvtdccel.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gxapumufx.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/graulitxs.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gsqmfmlam.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/goluwacgo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/guqzzybhe.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gfpjnkqyb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gzslfaaww.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/guolvjuee.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gvfltrfab.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/garzjeicy.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/grvadbdsw.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gpunekbli.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/guwwjrwqc.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gcimahgor.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gvsdyaczc.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/ghdehmdbb.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/geitwzohh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gjawlktgs.sHtML


<!-- 参考信息 -->