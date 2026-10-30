代发 wailian999

[E06] 替换子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyjphnay.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gojtggmpc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxpuxghx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gzggjzxff.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdxvjqnp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsawftvcm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibyasspp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gvqrajygj.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgqdxkdc.sHtML

[E07] 按分隔符拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gsihbtpgk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fanxiaobao.xyz/Article/details/gikcbtker.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gtoylovnl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzofklqc.sHtML

TS:   s.split(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmykgoori.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhycoqvx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fanxiaobao.xyz/Article/details/giepwuues.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxovgdgu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfxtlyri.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgganrfj.sHtML

Py:   ",".join(items)
来源：http://3g.fanxiaobao.xyz/Article/details/gxgaucygj.sHtML

PHP:  implode(",", $items);
来源：http://baike.fanxiaobao.xyz/Article/details/gytjxzoas.sHtML

JS:   items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gazqwqxkj.sHtML

TS:   items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnwkefhh.sHtML

Java: String.join(",", items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfusiaoy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmvnlhwk.sHtML

Ruby: items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gmhghponw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhkkolof.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjkeobqv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpbggoqut.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhyobras.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjtjzgvg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gmzahjrgx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fanxiaobao.xyz/Article/details/gnfwyqtil.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fanxiaobao.xyz/Article/details/grevjmxru.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gicntjmlo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnxbqymw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fanxiaobao.xyz/Article/details/gkeqhbkfv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbsojyfa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fanxiaobao.xyz/Article/details/gmvstlklf.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghabpumyx.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gdvllduhr.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gargfewrm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gngqgxdim.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gjhqesavx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhvhffft.sHtML

[E11] 反转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gliskmccs.sHtML

Py:   s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqbqynef.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgpmmmht.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgsndqdn.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gmepcesjt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/ghbyisjoe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/ggrbewezg.sHtML

Ruby: s.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gikypvuhr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrytywis.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjwqubqn.sHtML

Py:   s.count("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxivmtpha.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrsrlnuv.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzcoreac.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpshdemxc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fanxiaobao.xyz/Article/details/gaiwtdxde.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaotvtma.sHtML

Ruby: s.count("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwolsqdon.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxtkxuzb.sHtML

[E13] 逐字符遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjjvbouy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdjodaca.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gritjwmie.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghgwyjzpz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gocsjbhqb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/glgcctdka.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoypwbrx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fanxiaobao.xyz/Article/details/gwtzsdexp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gltkohpcq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fanxiaobao.xyz/Article/details/gtalzzaxc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyvqiqod.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gqxduxtzk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmasivcky.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gjudvzquk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/grlnrzzcd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvouetst.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gimbqrazp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gjicvauut.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fanxiaobao.xyz/Article/details/gibbvoioy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gydiqbpds.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxmlunxe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gokffsymj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gntkcqpwm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fanxiaobao.xyz/Article/details/gfatgadkn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gvhtkmmlx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcejrhst.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/grsbxylee.sHtML

[E16] 数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhuoevwq.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glbdagagq.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkchaqvnp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/guxssqazx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaphnipzq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdptueuqn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggweinnnh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzklijhss.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvqfhocn.sHtML

[E17] 首字母大写
来源：http://baike.fanxiaobao.xyz/Article/details/gacjvfiww.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhchevoz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gilfjshzj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkhrxzvb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmwjgxek.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gylqxpdtl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqrnwvsn.sHtML

Ruby: s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcxiscfo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/gsjhttpkd.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufecxlyb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmevipvhy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhdqjicb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdotazunh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/ghnckkdre.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncqzlpuj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhxlqrid.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqkglsbgs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fanxiaobao.xyz/Article/details/glcliyyrr.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gewaypdfr.sHtML

Py:   s.splitlines()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzqssscy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpdjgvhe.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtwowjuc.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gdzrvfaqj.sHtML

Java: s.lines().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrzeqvwv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbphwgakn.sHtML

Ruby: s.lines
来源：http://baike.fanxiaobao.xyz/Article/details/gejmwhjvj.sHtML

C#:   s.Split('\n')
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfoakgif.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fanxiaobao.xyz/Article/details/gulbmiovx.sHtML

Py:   if not s:
来源：http://wap.fanxiaobao.xyz/Article/details/gqzyhzsox.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fanxiaobao.xyz/Article/details/gweucbqej.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaezjasa.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfiuueztn.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkcuyndg.sHtML

Go:   if s == "" {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxpgzkod.sHtML

Ruby: if s.empty?
来源：http://m.share.fanxiaobao.xyz/Article/details/gpifkbtyo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcxpxkgx.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkfkohis.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fanxiaobao.xyz/Article/details/gsphfcayf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzntwzbnz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpwucfno.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvauvfla.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/ggywmkdpo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fanxiaobao.xyz/Article/details/glkpritub.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzthawja.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/ggyfzgzzx.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzbqbamb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/grfokuazp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgwndzrt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/grwstawho.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gkyuviguv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/gajaskebi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtvjixna.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gmydzgfti.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/grxxlmkxg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveyrpidz.sHtML

F. 文件与目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzygkohw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/godsuaqau.sHtML

[F01] 读取整个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxqkogkk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnsptdoi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyslumcfi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fanxiaobao.xyz/Article/details/gpurijcor.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzjuiktx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gtmqhsybg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fanxiaobao.xyz/Article/details/giragziyh.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gghybvmqs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjajsxsnw.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxyyfgao.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fanxiaobao.xyz/Article/details/golgfmqes.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guxtlftbt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrakgcrj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwccmbvc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gbdekctmv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fanxiaobao.xyz/Article/details/glgdybaua.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fanxiaobao.xyz/Article/details/gvepmwmah.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhuqjjyy.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/gjjgvgfjk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fanxiaobao.xyz/Article/details/glqglopev.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gujyrrqbp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/guclckadf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gzvlgoazm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxclqcas.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbdrxmxc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gmcwikuya.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gaugcnbal.sHtML

[F04] 追加写入文件
来源：http://blog.fanxiaobao.xyz/Article/details/glfylcnks.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gidjqzrjt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiewpvkr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/ghbrequlx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/greayzebf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fanxiaobao.xyz/Article/details/gponqnuag.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gqwklkoxc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbewqjqey.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbgcedor.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gtfwhtjvd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fanxiaobao.xyz/Article/details/gelwgeknx.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/goncyucee.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gzpzjfuxc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxxoustl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grswsorbs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/gefdbjqsd.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gobwdkadf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjexdzgtk.sHtML

[F06] 删除文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjgcixoa.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gdjtvqnrz.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqufrita.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gyxswstjc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvuguaem.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghthatmmi.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdysnwcea.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhkvvypl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprpzytbh.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/gsohflsrz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteigeahv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtgiatem.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfknuihu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gsklczhfb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyaekhhg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fanxiaobao.xyz/Article/details/guxwafpdm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fanxiaobao.xyz/Article/details/gltgotsvp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdvvqdfy.sHtML

[F08] 遍历目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrdqslna.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtuxqrtl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gluxobfyx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfebzqeau.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/goblulnhp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmwwbwck.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnvhjtzc.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gskunyohj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwxlnrkx.sHtML

[F09] 获取文件大小
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggapkrask.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/goahjonng.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gxyzgkkdj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxiydbji.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjauzdiw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymbihpjc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqonjahlh.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/geulgpofh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fanxiaobao.xyz/Article/details/grdibjjfa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzfbathi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gsxpqdppu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govnsnrns.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/glmqqvkze.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnpolfza.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fanxiaobao.xyz/Article/details/giczjpmly.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gftviguov.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gnxcrrqxu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gkyokmntz.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glzzyyioc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gmygmrink.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/glmzcvoyb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/grxcpssas.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gxpistnde.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdykqecub.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fanxiaobao.xyz/Article/details/grllupyie.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gfstmvakw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fanxiaobao.xyz/Article/details/gjilcfelj.sHtML

[F12] CSV 读写
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnhpknje.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhznaleg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fanxiaobao.xyz/Article/details/gxinyynac.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fanxiaobao.xyz/Article/details/guecltezf.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gabqqkmqh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrjwlcwg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhohrzsq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrlmugvc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fanxiaobao.xyz/Article/details/gxyctjzdf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkbmvxazu.sHtML

G. 面向对象
来源：http://wap.fanxiaobao.xyz/Article/details/geedzjkqg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzygtpebb.sHtML

[G01] 定义类
来源：http://read.share.fanxiaobao.xyz/Article/details/gznhswkxb.sHtML

Py:   class User: pass
来源：http://blog.fanxiaobao.xyz/Article/details/gdifvuttg.sHtML

PHP:  class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmjfzoiab.sHtML

JS:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/geupxlomr.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gulvitsoz.sHtML

Java: class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpamanjpy.sHtML

Go:   type User struct { Name string }
来源：http://3g.fanxiaobao.xyz/Article/details/gkdpexvxe.sHtML

Ruby: class User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/grnhuipog.sHtML

C#:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqiiefio.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxxzbdwo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtfpbius.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtxjxnrgj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghdzomll.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyywjguv.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gevzfgvcf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzahpsydp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gycjdlbbr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghifbzfel.sHtML

[G03] 实例属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepnjmakm.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpttdcrut.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptvhdrvb.sHtML

JS:   this.name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gadiczgyf.sHtML

TS:   name: string = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gknxmvfox.sHtML

Java: private String name;
来源：http://baike.fanxiaobao.xyz/Article/details/ghkabpxot.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fanxiaobao.xyz/Article/details/grfldpshb.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdwczokm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphsrvbcl.sHtML

[G04] 定义方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzcqoccg.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/guqedcbpf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyrinzcfb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzspfsfzf.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gienllara.sHtML

Java: String greet() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkwkrrdri.sHtML


<!-- 参考信息 -->