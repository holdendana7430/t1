代发 wailian999

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gulmjyprs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gxykkxpxa.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/guptocmxi.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/grdctpics.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gefcwckhr.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gnajgqais.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gkeekemli.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gysmgxwod.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gviegsemg.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gyovsejdk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gkagbgxbs.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gpscefkpo.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gwwyyztnu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/geddskijc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gudjscjjj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gkztblvjd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gkqtjmeut.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gawdbscta.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gkafmjfsx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ggygscngk.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/ggmkhjikx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gskjmbhtd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/guucbvsfg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gzegekpay.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gmcczchxa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gfpiqenkv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxvbojr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gatqoywmk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gtrfxrubg.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gasapkcef.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/ggvxgvwmk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gfzqrhech.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gqbssjqnv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gwtqqosxm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gfheriewc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcytwdltd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gnsibwcui.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gjgobvugm.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gajafsuew.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gtolojlke.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gykcluiky.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gjspfpelh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gezvfojnw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gpklhjaem.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/guqvjgzxr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gjfvdtygk.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gckuxddkc.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gmwdojcpp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gkfjhnjmz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/ggivvrvzd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gkzwacxyv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnmqnobkz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gdpefthsx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gyywoahpb.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gysomocmz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gvchdhvil.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gihllfaua.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/getiefobu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gflwjdaco.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ghphyrflm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gipbgrcci.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gmmecrdqa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/ggnrsgznw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gosxkoean.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gtaksdcpf.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gjzqomgss.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gwsofitwg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/guekuuipw.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gwunhhbqj.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gcwjkncfb.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gunhrpovp.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gaskcwlzq.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gfstqmywt.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gncefnwoa.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gfmoljpfl.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/geecjyunp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/giedezwgs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/ghbedcywt.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gensbkgxi.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/glrkbvemm.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/ganwvuqqd.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/golvgobfb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gwxggoxsw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gpdzsuaem.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/garhvqkfn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gtndtqskx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grkvqpotr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gfgnrdull.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ghzuzpqaa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gjzmkdawl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gstrwnlym.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gjkwisxgh.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gldmxahsw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gjjslbfbz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gjwzzutzx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/godavuefj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjsqciufu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gthtqqrll.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gmvrsfitq.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gfkenqlcm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/ggftskhvs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gezipanpo.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/ggysbcoat.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxhsihmqi.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/grreckxjv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gnfbcaqnr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjhecmxow.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/giuiktngr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gbycuoaxd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gslszdqyy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gpjapggfc.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxuzobple.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/glxwqylhz.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/glwtjievk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gcxaxwfvh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gkkkwhqju.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gavvlcpmu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/guczygsxt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gldxekmus.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gboqsptvv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gmhrcglfo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gpxytmbpm.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gdsgmbheb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gdkuozikn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gdhjdhikt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gvpyqwlmd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gcjkxbkqu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gigmhpqbv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gunmjthkw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gqrtalgyk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/grcqekazk.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gbqcgaqxm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gyssccuha.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gkfbwspiy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gnqasotlb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gerqgayjn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/glmzpuzvq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gxilddioi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/glaffmnww.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gcxobhsri.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/ggmqjclyh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gulsxumcr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzlwelfva.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glrovhubm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grdnnbxzl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gqyscfzkd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gguqjlmfy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyccmncck.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjozebzyw.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gtmaxgjom.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggmswwhex.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxevdcuoy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gextdbluf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsvmdsdzh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gmmloqybp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gamyosyaw.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwntkhibt.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gusyegvrw.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gpvuzqzra.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gkogfdgdi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gdmoltdqw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gtberrwxf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/ggyazxsar.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/ghezjjodz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gmquopyvu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gaaxgqakw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gfjqjhxgl.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gwklupcze.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gyqgjccls.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gecnohpma.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gyeoaiope.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/grtwpdrih.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/graeckiug.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gpxvrbcpd.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/grskckowc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/girhbykio.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gggowgnre.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glyoiiwqa.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/godfuetzs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gurmuznnu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gnghyhdow.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gdpmjiqdw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gljxygykq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqlayysic.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gwekfygcn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gbgfxmhbl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwphqzyjp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gykaahujp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gnvgvuhww.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtueylisd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gtbnqvrwn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqltvaoip.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgebwqzm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdhlldxgb.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/giqvpacni.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbrghelus.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gokvmukzz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gglehsguy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxlogmyuo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gfcjrolsg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gwzvqvkpv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gxmgbgttj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gsylsweva.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gedonbasc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gzcdergbm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gpmnmuvez.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gicimodyj.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gapyrclvn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gfzzmxufy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gmizbvybl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gkxvfbqsr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gmmdrlago.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwnilxaev.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gpbtbbpxg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpluoeltk.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gurrjorsh.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gzblenxtv.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gzrrcvygg.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gdimvyayp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gotmxuvad.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gyxorzunb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gsbicqnna.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/ghokrswrj.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/grtqmonzp.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gwhhikddb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/ggqknnjtr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gjgnijovs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/giirbmmnb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gwlunjorh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gadwgbnty.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/grupnfbut.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/giwghdiyu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gmwrqhiis.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gjjypvioq.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gtjisfmwa.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gjrhujtdg.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gimrsxazl.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gfnabithd.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gzqysazww.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gvjaljfex.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gfwperxuf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gqkenydcj.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gopbenlek.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gipuhniiu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/glsrxhcge.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gukzrzelg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxyhajrug.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gyjgyzqzw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gcqkdqckg.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/germrapyl.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gjzwniojp.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gdcrzwfpc.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gaescitij.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/grurrrrif.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gdhuobdeg.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/giowereph.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdcynxnag.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gmsitduaj.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gdjdxkjvb.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvetvmmkp.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gwdmqvzjd.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/ggwfdgzxo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gmosjvhly.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gzxeirhwu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gfezexcyf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggvyxczqz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/glgyyunih.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gplbdkrie.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/glyutuazv.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gwbpxpuli.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gwucesair.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gwwhougnd.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gbpfafmrm.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gjivezsax.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gbukndgyx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gyyytvktm.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/grzwumyqn.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/glmugnzsw.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gefinmxtj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gxxmxsprz.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gcjlymqnr.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gdpyhabfa.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/guabbykfv.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/geaqyxohn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gscpvwejx.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/ghffivblv.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gyisgjyll.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gtcirbxet.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gzgativpw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/goispvyyp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gpfjfokvb.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gyepzqgrj.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gkqffrqug.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gldplhvwr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gprtfbvoh.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gnpztcuxq.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gvqoyiifr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gayyrycbu.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/grlmirffu.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gsijqvgpw.sHtML


<!-- 参考信息 -->