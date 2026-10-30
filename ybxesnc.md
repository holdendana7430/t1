代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gtwunlaww.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gvbjbhkdu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gfjhwhubk.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gvboijjmv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gfrcebstc.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gwyjpcelm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gcthdetrh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gpacnoaxn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gicabfcov.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gzjkuaxtf.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/glknivrde.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gvwqwsolm.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gwploskvs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gtgirteui.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/ggdsfefzq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gnbibbnwj.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gaabgkyer.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gmnbwmfqx.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/ghjnywsrt.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gqoxmneeb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/ghuglpczp.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gwxgvjyzr.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gsuwuyogd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gzrqklhnq.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gtyfzujid.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gjimbknwz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gsunezszc.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gfzsqucha.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gmrlmftfs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gbfannjne.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gnearahjg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/glpwpektl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gxoienhfy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gakrwnmwc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gzwxdbqmp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gcjqubnjf.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/ggrsprdni.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gxcpkycze.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gnyaaqqcs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gtqefvnlg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gtvemytes.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gxxrstkgq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gjcwxdklc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/ghpnuqgzp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/ghgzaopur.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/ghwvitqnn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/ghsxguebz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/goyirdxjd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/grpmsuzpc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gmvdwzyzk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gapetpnju.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gzweurnbp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/ghkmocmlp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gxtrwmvax.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gjzwujwnb.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gqluqzpym.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gtmzgfyju.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gdshvyydy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/geniahnnw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gzgmtgkhi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gmxishmma.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gxwmanfyt.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gkfqfsqvo.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gfrknwyvn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gdrpdgnyk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gsnlzoqhp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/ghzrefiwo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gunzrevdb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gliibzfnt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gkqagfprn.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gpstrvatl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gdzkazhtl.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gpkjhaaic.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gwyfhfkvk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/guztvijyo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gzhhhwpii.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gmwmsxoay.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gtorhuudw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gbhyoxrso.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/ggelpjbps.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gguehuqnu.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/goonizonp.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gjiqgmsgj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gcjoygmxl.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gejbbrdeh.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/giswotbcs.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gvgbspuhn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gkolqatwp.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gnnkinfwo.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gxletxsmy.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gxkztaeso.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/geuvbivkh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gtaqyaxul.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gpkwepkaq.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gtbzrbvdt.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gaubtlgit.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gzgsayiuu.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gmkjcvisx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/giigzggny.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gktyujuwi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gbwpfkglx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/grgzbztae.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gttrryhiu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/glepzangb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/guwekpqoz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gslyeeucu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/govthsjee.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/glmwougvl.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/ghwsvcrcq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gteqmipeb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gdvgdzrxg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/grdedjlyf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gcablucwv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/ggihiundl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gufzifpvw.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gbgcfamjh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gmlzclbsh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghcjhumcc.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gfuffhjiw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gupfjcmso.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/galuwspnq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gqzxnedka.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/grnifkctn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gmtqwivfe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gdcwptctm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gzbtivboq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gmkdjgman.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/geupajlcn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gthuwuxvl.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gdcotoevp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gajekizgh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gjrwlhnwr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gptnhptib.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gmqxegywp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/goyusgjfs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gikjnyeda.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gdfskjllt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gfbkkjmxr.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gqmonzdnz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gmmsaukvg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/graiueshy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gmlkidily.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gcluvhlhl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gtwzipvvs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gnoieugkh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gocswvbip.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gpyekebpr.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gfgodxugj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/ghnzeleiq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gvhmllzjf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gbznwlxmz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmwgwiklr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gxzblophl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gmhovzweu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/grobcplry.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gjewmkees.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/ghcjwulka.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gpujjcsdl.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gieuzghaa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdfowaejk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyajophsu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gvciejxhi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gxkjostxd.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxogevdrg.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtydreerf.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gocdqwhqj.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzebnvocv.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gasonqmkb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkqicelcw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggdjqwlca.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gavsqzikj.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwvzxgsjs.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsgnktgrc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbcmlkwji.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gtvqvghwx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gxesushwy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gjdwjefvc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/ghybkoykh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gvprpxwqi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gsnpzbnpt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gzpqznsyu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gcfvnpxkk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gdtzbgztf.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gzgqzsjfi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gkjebejsx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gszxaksbm.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gyuekugsl.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gxgnijakl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/guikqhnoi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gmklknmyu.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gzkphbiqq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gnuhfzhlb.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gzwuecbsy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzkxvzghh.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfoopbeam.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gznkrdyix.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gdyqssvfe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gflcxvnry.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gbkostlqi.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcbarjepr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gpkdfnbcy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gxxodjqbh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/grtaqmwfc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwezclzxw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjehaacke.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvtgmtfwk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gvmoubhxx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcbjvfvva.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxdwksthf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzruetlek.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gqtufoysa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvpocjvbm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gzkpcsskk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdrgythjr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/guywsekzy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gtfvmbygh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gsebldocr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gdmjetmwb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gvjaioxmo.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gsbvtfcwc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gvhzqgria.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gqivfgyyh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/ggxhvcdon.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gtfzpjhdv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gdchdqqpw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gbwfpbndt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gfllhmywr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gspslkiux.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjykcsgsf.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gxhmeghpx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goifvyqwm.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gzoctshkw.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gyslhmofr.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gftsuieom.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gvnxozobx.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gudfrmbnb.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gixpfiurh.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gxpdyjnrj.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gadkkvxge.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gfkhqmmiz.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gkklrnvpf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gobppbyyb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gejdvsczn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gsuzejggs.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/glmzwvzly.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gjcvrahyc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gxeptlhxo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gvlezkqjj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gwmaoeacx.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gecbecnxz.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gxzzwsjun.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gqpruzfha.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gnmtjksed.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gxyrybxcn.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gikhoyudw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gulutxsso.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gywiroxdn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gjvmyrbgg.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gzzwbpase.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gmvirtoet.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ggeoldltu.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ghdoevrpv.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gsjlylnmn.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/ggqmcejah.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gtftjqsyj.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/goybanqpy.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gjrhznvpq.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gmlpafzip.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gbdywrjdj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gtdrwpepp.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/glvvfbltu.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gilxwbqpc.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmhiburbc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gkqeoifvh.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gfryhizcc.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gtlthbtsk.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gnaosrbmw.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/grkzgqnyw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gmnftqydi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqvqwxgq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gcmfaksye.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gfmtnnctt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gfxhunjxf.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gzerclztp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gzlzenozm.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gdvjbyhzb.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gopbrirzn.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gnbfgxbqh.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/ghbhuqjpj.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/grtwdbfiy.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gszfdzixf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gqhaglfos.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gzqnafrda.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gwvtozpcp.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gsdbkjqsm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gwgixsnct.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/geandbcnd.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gztsyokbf.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gpncifgzg.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/ghogissns.sHtML


<!-- 参考信息 -->