代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/grklaavou.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gokodajip.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/glicvuzmt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gvfpabyeg.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gtralzxcq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/giuyujfyp.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gcqaessni.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gnsrhdksh.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gggzawvte.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gcowtfhns.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/govdydzjv.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gwtsolkvv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/glhcgfrlj.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gwwbzrpkd.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gdmfmiwpc.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gdujsgvav.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gylmjyjvn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gynolrtij.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gjvtuknfr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gfytqulgf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gzrwafmah.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gytjozwnp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gzvnygmnu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/glbltoxti.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gfiyxzkoe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gaaesyrrt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gtlhxqddv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gukimfmtp.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gkskpcwqr.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gmfdbkjui.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gvczsjdbn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gzutbhqnh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/ghlvjzror.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvuxidh.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gomrazpyv.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/ghpncpwjq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcmakkosh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/goxaehfrf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gjiszjqlu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gpwhpmbbb.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gcavgcfmp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gwqjaggmx.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gajqbtqqi.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gqorwggxb.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gkkzfpbkl.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gcepfdadx.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gjfhkcrlg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gtdsadqhd.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gbsjhdibv.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gkhgmyynm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gngxdsgee.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gbpzjmqco.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gmjedplve.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gkljorgzi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gyajiaguo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gnukwqivf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gfpvzwjsp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gyrzinqzc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/geyomdygg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gaayrrmbe.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gurfszjgv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gqafbvqdt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gncuwxdyi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/ggmrfssct.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gyneiuama.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gzotdnhnr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/guycicumw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gbbsmjqgz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gpbcdvtkv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/guzxmcavz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gchreuoyu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gqksrwerj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gredfyibh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/ggkzuepif.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gwqynevop.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gdwfwpggc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gjxwazxai.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gczebejqm.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gauckpqut.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gglldewpa.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gtzoxdosg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gbhgofiov.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gtwwoprlq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gerlrzllu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/ggqomgsva.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/giejubhpn.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gffdhmqke.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gwylmfywv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gouorxlat.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gjlzqqmer.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gxximasqs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grrevspmp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gqzrpxghj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gcjcwoibo.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gmprofjmk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gcltwzotu.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gwvkwgnht.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gvytgxlfb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gvxjlafpa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gnqjoavjt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/glgprkrgc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gakzhctou.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gexdhduuw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gysxeqrmi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gyfaywxqw.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gkifqiutd.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/girqjcpri.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkzbixkpd.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gsuuitjoc.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gmoccppga.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gzrupsvtk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gpqhotwkv.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/geqieppwn.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/goychhumg.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gchqzlbjc.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gyueeqcyc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gywlftosk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gywpppvzj.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gcukpsopn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gqhsuaiae.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gbfqqewut.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/glpwyuzyo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gwllzupis.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gftonrqtc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/giyzrcjxo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gxpzhoimp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grsdquayj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/givevbfol.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gbamyrpgx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gfxpmuxtw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjfnidkmo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gljrjkhwn.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gqcwvkpja.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gmakfampz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gaahsocis.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gpardywaw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gflzjedwp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gpoeujsjg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/guvewehnl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gqyzacbnh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gmwsaegsa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyfwseguc.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gvrxmlrmu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwzgzqfga.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gzuegdyxg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gdihhgwdl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gggsfevwh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gisqeyukc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gdgudwokg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gmerdcdhr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gknbgvlkh.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grktooqto.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gqzycrqex.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gyhemwuze.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/guprydvra.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gduqbykak.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/glbhakoxg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbgjbfwvd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gaiczyewn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gavtwlicl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gvnphjndo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gfwkkovjx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gkavmvoju.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gphecrpne.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gkttjcebh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gxkttjugl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gqnowecgf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gswyfriez.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/ggtkjdhuo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gpacsjqno.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gapcehshp.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gtizduaki.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gbhfuiseb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gaijikcey.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gscluumil.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gdgkmlpif.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/geqdktbwd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gnpwulmom.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/giayfeteh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gphihgche.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gtiumvvnb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/ggpmulmcd.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/ggskfogtw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghpomtpoi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbzcpnzcg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gtxblmmxx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/glufktium.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpyuiqjjz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gaujevkhn.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gbphdkvqd.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggamcelvz.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gohwigibh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvivixnro.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqwkxippp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gvieevgxo.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmartmmxa.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbtxucjhq.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjrtmyxfj.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gwxlzytcg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gzfupgpyn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gjigprczr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/geojcvkzl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gubywyuup.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/ggyhlbocy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gxdioxmeg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gryuokrad.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gclriqnqd.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gyeafruwm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/geerrcaop.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gwezxskqp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gefkqxcpu.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gateaugst.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/ggjpfytpn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gxsvdmwfb.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gesfjbmoy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gygpuwted.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gxiqxmqzs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glcgguuyu.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxidliphj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/glzvuocqz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gphbkejjx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gthsxhsof.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/guitxqnfb.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/ganpvmnby.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gtqzifpti.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gmxziiqaw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gajnsyjoq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/glokiyehp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gfaumromy.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsnayaset.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gvqcqeapz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gncxfefev.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjyslupuo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gppdszyrp.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gptkbgurn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gapgltxbs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gomoycfke.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsycathyy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxeflneha.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwuqcytr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gbkfubokj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwarreojr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gezqiljif.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gvwsqcrmq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gneytgcuj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/guilimlvh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gwypelmtf.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gtroefvvx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/glkaisdiq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gocqqqxps.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gxhnluecx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gqabphdgw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvgsajbpt.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gzmirzzkd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjgwemumt.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gbluntzzw.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gtowmpahf.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjwzxdoah.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gotaxxrks.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gfzmjkyaj.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gqkulpics.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gfbxfvkmo.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gqrsarndi.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gwarsnvgo.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/ggmbgjaco.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gyuokzolg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gbtinvrft.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/grrxmagmw.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gbrghpvjc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwzqcrfuc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gmxqdxgwf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gquzkpvga.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gvrulntch.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gypjbcoqg.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gazwxjnwi.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gvcpaihei.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/grgzexyai.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gjzyrumsk.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gksmjpkrt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/ghzrpmxdo.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/ghcqpdvut.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gszuubkre.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gvsxwckfq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gsieorekx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkuuwxsdt.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjuvkelmc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtojlaakq.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gzyclsenz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/guuzaqsmx.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/glqezvbnn.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gtvjfamrt.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gdbkkhrwo.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gqijwhjzd.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/giumfjyut.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gtkscinwy.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/glsghxmxk.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gibqjxqvk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gbqlrpyrn.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gybctbfge.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/girvbpizv.sHtML


<!-- 参考信息 -->