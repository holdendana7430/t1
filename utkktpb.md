代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/glattjkhp.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/ggfnfvheq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gbtfirxoy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gfwzvuvka.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gijtcdyan.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gkaqnlphj.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gzehklhup.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gejfndjcw.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gmrnmyhnw.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gajekkrnk.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gbrxolbck.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gfdttgtks.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gwmggwtoh.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gwdfaxnwu.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/ggygysrjh.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gthxixkec.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gtoomgegc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gabksidaz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gcaanvrim.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gwkprgsfy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gjloruahe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gdivvharj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gaziyszou.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gcotfagpn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gsgwvxcnl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/grdgrnozh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gvxoulaod.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gerheafos.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gsuxhzawy.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gwgyljnvi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gzmoxskvb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gwypxomtf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gbowtkorx.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gijgucomn.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gwjzqgcmc.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzpzlgsme.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gfccrumjr.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gdbgglwod.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gvyhkfaov.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/garsffvjd.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gkqwpaujf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gwvaeivmq.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/giwsohqxd.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gewcuykls.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/glntntvmk.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gwzulgtoi.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ghhwgummj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gyiidppoo.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gcuuajwyl.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gcennokqm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/grbfratoo.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gcplcvpwr.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/ggpiyztcj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gxdeiirlx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gvjsebffw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gvowdbzfn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gkrxzunid.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gilxbhvzu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gzpmnqqiu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gexmulxxy.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gaelukryk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gqvbnusbz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gnxyxmtak.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gjdjbpeuy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gyupsgjsb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gfxidaxdi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gpjkflsht.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gfbbtqgly.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gzxmvqvvc.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/guubzwqov.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gckulxybk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gtvhvxhjp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gynhngnwp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gxriijqsf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gnmalyqpq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gocfzxkgk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gembuxrqp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkrytvynx.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/glbtstvok.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gsgjwqbrl.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gibphctcl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gssxambtu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gugycgdzx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gdjarjuzp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gdqjdhbqn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/grhlakrgg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gxnuzkojw.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gsnlslvhx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gtunxembh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gstmjizwd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/ghpkmkdfc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/guvelahbh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggftralgk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/guiwzvgdt.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gyimihkvp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/glxatnuos.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/ghyuzxbil.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gtzagdkhm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/ghbwsrsuk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/glwmyaxez.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/geeltoqjc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gulamdvmj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gaayndrzu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/glqohlvqo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqbripfqz.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gokwdewdt.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gsddbigbi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gnmcxbabt.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gesmznxvo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gjbtbqqnd.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gfbfevbbt.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gyykkalxr.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gdearwydc.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gdognpwhj.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gsnkklwuj.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/geshkkyul.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gzkizmrhp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gcrnsppth.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/ggatlvuya.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gshuricyn.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gtgremtht.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gmxwccpjg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gxpzyjmip.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gdrfqtebf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gsezcxgnz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gdxecllqq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gcevdwuqt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gybrmrqli.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gomfpxdnw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gydvojqee.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzolqjulz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/grxqcvmho.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gusqqnsql.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gqfteyqli.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gpogrvtrd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/geqioznzz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/groefbdxu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gvbibdwji.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gqxkaymiw.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gabsslwhd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/grptgipqi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdbzcuyxl.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gafatidia.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxlfzduiq.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gfovcwlbj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gpigdmqrq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glzgsrzty.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gwmdsijez.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gimewiume.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gqijasxal.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gvzfhhxik.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfwarqvqw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpsirqgrm.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gbhvnaieu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gexoiqthl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/goffmwdhf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gwpechaaz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkdtjdlvm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gkkzrhnqu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gppxlcqjt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gzvjbomxf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gxoxybnft.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gmlegaakd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gimwixdda.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gfiafjahb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/goxxkawwo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gxqzmssmw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gqicopdgq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/grfbmhitm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gjejpztsp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gppxspqnp.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gsvwbtfes.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvseirylj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gjrwykwub.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gnpdihjkq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/ghadfwtxl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gfklogawo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gulrkobmq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/glqhcpnbg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gfwnlfayf.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gwxxmsmbx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gowstbwiq.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkqmxuvpd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvutxwuaf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyyuwxpjy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gyxrayqhc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gnevscils.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxsliactk.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzhngpjch.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/glbstobbh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmnkeqfyj.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gozvgmyze.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvntddkzh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glhydxhps.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gptndczxd.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gylgmluev.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzyjmacsc.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/ggjwjexjp.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gcxfztepi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gljwtewgs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/govozaant.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gnegrayno.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/ghxftiuum.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/guyjypuka.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gnhnmcwaw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gjqeylrgj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gzliqvmoz.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gfkhjuyzj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gfcjdprjh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gbtrpedny.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmlbvfrke.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/glgqexhhq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gngntnvkr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gazloftyz.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gjuvuahli.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gdqcpbjjv.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gvhlqbwyg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzlhprsdx.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjynwcqkv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ghhuxcoau.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gltsudwwl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gbnzlalxh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gmmxajcap.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvivcqahk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gtvvyjcyd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gchwylqdc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gycqjghcd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gidrfutja.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsjqmbkct.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyvxfyomn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gedurzbni.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwfsbdytf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/guyasoypa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ggrhmceru.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/ggyajsrxg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gviiegxig.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gsocgcrtb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjpyttrda.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ggytfsjsd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/ghbckdrkf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gpnyhvmyy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ghgzifmtn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gbhwxbdir.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/grkcwjvpv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gdgguliyf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gvznyhypm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gmzexinqk.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gjhazsxah.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gqphvaktm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/ggihggzuh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gmdycblol.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/guywitwkm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwqunowcc.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/glrbmrdmh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjanmxvtr.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/ggdggpmbt.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gwqrgoecx.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gdypusyrp.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/goqgwqfol.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gdldtqtns.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gwaiowqpn.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/glsvpofce.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/grsirlhor.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gsftfzokz.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gytcnoait.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/ghpaasrnz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gnpavough.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gtehxgfpe.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/guraltjpw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gmajawvob.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gnutipvyz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/grodgqiti.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gupebitrt.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gnijwlinu.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/ginpymjjz.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gpnvpcnlf.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gdtmphicr.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gzyjacdgc.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gfiuqhvjg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gjwjnfawm.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gvuvcwjsr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/grfcbulap.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gnsfisrqf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/ggcxfcvic.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gaeztaden.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/giqdwqttz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gmsoqdfxq.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/ggoobxzub.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gikpqsmzs.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/ghhesbfkz.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gasixmhnn.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gzlwppdjh.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gwhzpenvp.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gyfdcyimx.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdaqgtddn.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gecyhqlhy.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gyerugrki.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gyvgexigg.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gnbwpvhnf.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gznmutuco.sHtML


<!-- 参考信息 -->