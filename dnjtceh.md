代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/ghdrdidmo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gdoodxcke.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gsyzhxstj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/grfuleovo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/galufbfcl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/goqtyirxj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gxtqzlwwv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gexlxwmcg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gtqixquix.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/grxdghmtn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gexfohxtf.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gcjwovcmv.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gjpuywuoa.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gfbnpdobx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gzmrnoxqc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gskzlokjh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gdaacoyxv.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gpjdhehad.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gyqquulcb.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gaoqeyzxg.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gcidfrsba.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/grmllawli.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gneziijvy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gdeptcmza.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gwlzymmiq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gggaqmtkn.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gpbrdvywq.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gvbpjsnuc.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gjpezkmfj.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/getoiqdtw.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/glpytkbav.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gsbeicvqt.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gkayhtmav.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gyxcgxfbk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gesggpmlu.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gwestdddu.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/grpucvnpl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gvdfqgxtg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gfeabbmzv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ginqeilui.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gmbswjqee.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/ghpfgjyjd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gbdpepjkl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyvfaowfy.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/geiynjmue.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gdoskemcj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gjiqlitjd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gbfzzlcva.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gesurnivs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gcjgiwrfr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gvfbdrele.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gtpyonybm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gcoukrord.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gvqozeexz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqhgqmffg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gtewvdgsh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/ggmbecrrk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gaykizknd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gbwgbxwuw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/ghbwyimft.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gmhlgwcpp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/geqaplnwv.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/guwtduase.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gbxdvdcxk.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gruujkwms.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbbrvjjx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gbiazsczg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gegcsicdq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gmhmpstpm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gjalqeexa.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gcypczrhi.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gsytsorvf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gvttlgseg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gxbzklfow.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzefrdinr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gxykbpmlg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gaqlowifq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gxinrnjgp.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gmnbdfpuu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gjrxzbghj.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gszlhjgkm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/grvjzxvbv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gzksxgwyk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gvohhfpov.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ggdsxskzk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gamhalggp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/ghcwenfdp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gpvrqmvwh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gfjgjelqu.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gelprfswz.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gpukzfbdx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gkfugfjha.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/givnhkdzq.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gsbeejfph.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gshkbveqq.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gnheplwqn.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gyyfkoacn.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gqshqqrab.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gxjjwvgyd.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gjovmfhwi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gxhgrajvg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/ghjfjtdpi.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/ggzmevwja.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gqhsdtbgc.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gwqmzqtnp.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gnabshdsu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gtwwmtipa.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gqxzsvhfg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gkulswsyk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gvhcauxpv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gownjoisd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gcqmfplkz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gzdozbrgz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gbpmkbjsv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/glolxhyqz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gxukylyfg.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gjpuqnbnz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/grlyehqwz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gwhhlmjwb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gropbyokg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gjsesqhtj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gtdrzahjo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gogskyiuy.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/goziezwjw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gqvgfdtzv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghtcaetvq.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gwbugigek.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggqoghmvh.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/galyawlln.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/glixvfhcj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gljghfhjp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gaestbctb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gkuavewlf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gwzhkewfn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/ghfbiajsd.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpnbwkgiy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcryecqpt.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/ghfrxbiyz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gjrqswvra.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gpimrlluz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gogasxozn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gnrwyejgz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gsomivzbx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gfrvgiudg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gsxdsutdi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gmxgqyciv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gasntqrsl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gcxtaxryu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gbwpqsakh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gbebrqont.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gsypmeruk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gdsfvjwwy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/grzdmivjj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gewycifjr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gbemtuaay.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gtvymgkup.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gpcznbtpg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gumoxxxhx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gcassqgut.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gvhisxejf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gtczdbgel.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gqifiyicz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gsqkwjjvg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gwrxxsvru.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gnuhkattq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gubmfawed.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzrfrsvfg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gawzvlbsp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggwfeufkk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gmaercocq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gnsyihxgf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggoocbpuu.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsvzikirl.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gvlvtqxwd.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdrajdggm.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcpjbibdb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gaktwknft.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbwngigkn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ggftcirbx.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfvamhtjw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gppnxnozs.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfhvubynw.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gnjaxdnrq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gqvttdjba.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gnkjeypyq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gjnulvhiy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gexvhbcis.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gynxhbbch.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gfofjpjlb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gjnuttsku.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gwtfwcufg.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gjhjdptrv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gcxeyflsx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gvcnsscaw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gzkmtmnej.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gkazaqnhr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gfhyponwy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gulgzjhip.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gdaftcabt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gtusobgmi.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gkrdpbvwl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghomypqfm.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwabvhpne.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gfeogxcqk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gbqprnbha.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gjcdhiurp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gitqcjoio.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gknpiqijr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gwjlixynm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gstokpdmf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ghxybnzmv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gkyujzycx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gpyspzccr.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gaaqbtlpa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gdpeuckyu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnwihpvey.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gblxlbsrt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goikrjbon.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gjketybfo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkslfyxmg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpkdvzfvv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gxmpbcsup.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjpxlcioz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gghmdzqkx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gquomxtni.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gvhhrvpos.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gxesqdzzv.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gazqtrbjr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/ggbqlvicx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gvmcxskbh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/geplskujc.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/goijtzzjm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/ghtgyudmo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gyupnvayq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gbyqwsobw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gdobtjcsv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtbiwyhff.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gckcuyxch.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grdkcydfn.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gwkhffcmo.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gzgoiobfh.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gdtsdukvc.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gujyfklxk.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gdjxiphqz.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gylfhjlgv.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gdhgethtv.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gpzryyepd.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gzdbvsbdo.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/grtovvblq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gcbiyyhkw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gesdyrkhs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gtnlanvug.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/guzpftnkv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gigdahfgw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gudjjllmc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/glxlygnsm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/ghqpmwsce.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gmvzaatcf.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gpxyshjun.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/glntkodrs.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gstqimypc.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gpqygdqjk.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gnrpudxsr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gdhlqapfb.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gohuewlaw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gnevzlslr.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gcwkpvlcr.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gpoxavwiy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gxvdgjkfr.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gyrxcccmk.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gogrogtuo.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/getjrfgft.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gtjjebtlq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gzglwxwmm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/giryrncqq.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gsmkvllvd.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gknehzvdf.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gwuyddynm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdgzbyynn.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gvygcggal.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gazohulcd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/ghvynvkdq.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gtddfgnua.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gdvwsdbbg.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/genjxprkn.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gqnlqdilz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gslnqmkwu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gqbnqkbtm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gvvtaszqv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gzserfdgu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/glqpaqnvh.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gcmpiyebp.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gwsokqedi.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gvnrqrsoc.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gvmfljzsm.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gyutapcbc.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gjrgwsxum.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/goyhxxtml.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/glkrmxvvd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/grnmwxepv.sHtML


<!-- 参考信息 -->