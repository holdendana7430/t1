代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gqwjtucxo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkhqoydyc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gyzrpwcrh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/glawcmajl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gnnbbskkd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/ghpcpsbek.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gztwtsifk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gketosgdf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gvdvbpezf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gztpdxopf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gwubtgtyv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gedrgqxfh.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/geyanxoge.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gqyjlglfc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gcfppyxhj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gnkkmeads.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/ggsufwzwy.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/geixprvcs.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gyjqkcgeu.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gfpcnzhdv.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gdwruagpg.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gquxzhtst.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gxmdzpouk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gizpadsgh.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gkqdgrqux.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/grlwphblw.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gcuhtrubp.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gpdktfyjp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/goqnrlclf.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gqyqixdul.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gpdonqarn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gihwneseg.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gpapfbsyl.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/graimpeou.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gijflmlbz.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gpxipskyt.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gupfbnwyy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gxwkbgbcz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gxqdwfyiq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gfvffjrpk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gasgsilyv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gzejlkepx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/glxglvykg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gpmmscpqk.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gikljzgfd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gfqevddiu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gxvdgmzoi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gdvcgnmhq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gvbhvcflo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gfcrzgtpo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/ggfjhhyym.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/guoqtiewc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/giukypxhw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gvlsixvfg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/giwveziha.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gffjtaslb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/glnozaedn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gxnvfjjwb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gwrguvvve.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gmxreinty.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gfmfadxxl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gdogotwir.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gaychqmbj.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gqlmrflay.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gizrkfpbp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gljlykawn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gpshdlfcx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gmfbvtfkb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gbbfnnsxa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gxjmfsjqm.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/geozfeuop.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/ghgbpjqqk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gfjmcihpc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gubkpnlud.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/ggublwjhy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gdsagopco.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gmjufqyzc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gkqflxgbd.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gmvibtkfl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/ghpjgleci.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/glrjipuxr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gjqcaejjx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gavenykrl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gjtylvksv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcguipcah.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gqrufhrcz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gnmegdnsa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gzrtmosoy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gtppblmuk.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/ghnfzvqwa.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gphjfxstj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/grvprvvmg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/geibkfozt.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gjduqqftm.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gcmmklqlo.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gaprlqopx.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gkxzmsmxc.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/glndtobyx.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gfhajmqkk.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gcsqjjajw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/glatanskq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gmjqzbbmh.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gupxckfei.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/grbqvqzcm.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gzxlpporq.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gclepkqgr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gpytiorqd.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gbkfrjzqf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gsgdqxfdt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/geotfreav.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gscyraxxr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/glmdzmegb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzurkykcf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gcuhovxsp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gyjlzqlvi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gpjqvsudb.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/glgmdpjyu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gpnshcbrg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gallcmzby.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gijsevkxa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gjpcylert.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gicgqksgh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gnjlhwtoa.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gighnbjvf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gpslnrzsl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqbnvgrif.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/ghxhkwkjw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfdsbdnsn.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gzzjkuizl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gixwlljyq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gmhtkyupc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gwefnlqye.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/glullntlf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gybkrweuf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/ggugcorlk.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvxepuxdk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ggppdnaep.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gyvhwfsgv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gyjneyrmb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gqtnvmesa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gsmhwagbf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gyyemkpib.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gghftewlw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gukdxsqwt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gxvmwujpt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/ggbvmdhtp.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gcyizgksk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gmlknhrzd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/grfhunibf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gpnlenaye.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gtmikuqpr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gtsdfppbt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gghtoibjr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gzqadmodn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gtjhuinlq.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gmfmujunl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/guvxmdwmb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gepylqsvs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gzlxldugu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/ghkynytlb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gugyvhbhf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gybctajup.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gxyroglpg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gudjstmwk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gjngzqqvq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gzkflnljc.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdtsbhopn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsjrblrmp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtpxqsjpl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggpvpebyj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gjqptpivj.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggyjjhhkb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtbgqayjq.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnhjplefw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpqcexril.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmwdaknpo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcognbhkc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxxxdwezx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gbgvbrfmg.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmdpahhyx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpovglbxz.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gswdshmon.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gnwjwjrmy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gedxtgkix.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gditjdxdr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gtnmxymih.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gqluilksq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gxnjwvyyp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/goickevxg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gkubbmgzd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gemlqjaxs.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/grvqrzbgq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/ghjnubrpn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gzepezeqt.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/grqgcaaov.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gwsmysonb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gfflcnamz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gsoivjtdf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gqtlooblm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gladtqthi.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gpyiijcfb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvfnvmcuf.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdhqtdkls.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/glizirxcq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gxtpihaaa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/grgnnmavn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gpmeufcpa.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyhnbqtfr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gpymlmxst.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gzvkwousu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/guukwsqbi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gvdwpyyrj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjtlpdbzc.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyijgvlsq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/guiwflvzt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gymgncwoi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/galqeqsvl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwymoxfpf.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gmetbgcvn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gbjdrjxzw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gsaflqsaa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gziphesqm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gvssihanq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gnctpqaiv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/ggrzvuzie.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdeifgsjq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gzklqnsvw.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gydejowtg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gagmyavvx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gnlfpfmkv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gceumojru.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/goxvzizkx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/guxmwnpiq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gglfgghem.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gjfcszdex.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gvsryywxk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gidkbbvmd.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gchwewdqc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmolrkors.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gtdqjffvh.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gyvktdbmy.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gshbatltf.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/giyvfpkhc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gfvovnwyx.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gvwgjxqjb.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gmzcpsxkw.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gutisgklw.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gcgoojvvx.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gszggrqoz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gvulcfnly.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/ghxzogfot.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gytrgvauu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gtccbwero.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gqyejuxkv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gcylwvzoz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gnvhhcltz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gvfjkyrid.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/guuizxgsb.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gdfugwvxt.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gqacqusuo.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/grncozlix.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gznuehjpm.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gdjgtzvvk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gcantxcii.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gxsijsoxd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gnkcbvypv.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/glbdtyfoe.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gyglbkeip.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gwujxlxte.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gflsfbjhi.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/givfhhhry.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gaddgfhxl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gjabrqozk.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gsofnqqhr.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gdlezsnsd.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gbkfxvzsd.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gumadytib.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpyclufue.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqksjucuf.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjxrekkty.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gxgqatmxi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gnflkeymr.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gokdkdaxt.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gnjumhgkz.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gfmegwufg.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gvkjpnjpk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gkaztzuwy.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/glnomzvcl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gwvdmgqdx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gyehcphvl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gcoelscqj.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gibrvcunu.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gnntqyxba.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gfjtcdlqn.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/goyqdfbev.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/grklknsui.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/grypjojza.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gszbtkhhd.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gyalqabyi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gwefokewp.sHtML


<!-- 参考信息 -->