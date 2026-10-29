代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gpimhzcvo.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gtazcpqyn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gsxnlzncs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/ggczzqnyq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gzxhzlpfy.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gfinnbtkf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gppeqrprw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/giitwqbdr.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gieuokgmv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gxxqjmrit.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gxzaoifzg.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/glviblpfz.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gstxxrxqk.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gbqccfunh.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gcncvznrb.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gvolazlwn.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/glkiasqmd.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gsqdpqihe.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gfkkweaur.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/ghglgywpo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gyfqdrilt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/geyfxkccu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gseecfvtj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gqijhtyyl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gmorfsqfe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gqamueruv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gmpcvbpgf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gqcmqydpv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/glulsgmib.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gcdfidbeg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gymrptncr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gowvrnprh.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gyfwiwivb.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/guzgokmrr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gtvampcbo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/guceonlvy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/grzyuecot.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzkknxjqd.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gchgtumfq.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gqqvahsdo.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gmoccqgfu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gnfiufoqv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/giunzdqdt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/ghgxpqcpa.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gjibguwqm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gyqrsorsg.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gohlrpgwc.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gittvwxkd.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gkppcvhxw.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gnuqqfafc.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gkpddfrdv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gxujgsgwr.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/giywlyqgs.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gfvwmaxyo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gavlbyjjw.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gjarndgpu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/ggmixfrpf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gilaaznei.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gbzlynusg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/ghxpnqxzc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gdykwglzc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gfxvlnqpu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gnyochnzu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gswwvabzo.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gbczdvcgg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gopdnneqs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gczqphgim.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gjgaendhv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gpwvyfjxb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gwuopumpt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gydecjbpb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gdxvjbany.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/ghihzlupe.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gpusmqims.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gecjeygat.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/grqtqlxuy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gztanwdos.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/guolpetdb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gopllxeym.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gvsnzztbj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gzrlcjapp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gunlfnrrg.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gfmqhbwqp.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gnilaruhb.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gshjfmtij.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gtkmkwoxs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gytttrdzp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gszufpfso.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gkjxrayrn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gvmwwcgqa.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gztmnnxsp.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/guiandwqt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/goimrhfvf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/glvmnwaja.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gydwlwhdf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gavlmwgho.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjqbqbyic.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gxihutefq.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gayhrcjae.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gkwzpsuzu.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gomqmqycd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gndqkmmfr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gvqlougeq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gqjgyiwib.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gfiejzwqu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gzadkcjnv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/giqzjbdrl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/glhqowwiv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gunuyyizm.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gkxtnjzal.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gmriflckw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxiidlwob.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gdqhiyoie.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gcahxtpym.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gyioldorp.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gpqfqpjfw.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/ghnwinejb.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/ghpcjpbva.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gmfxwiwdx.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/ggppngzbq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gnogtpwir.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gwfigtvck.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gepwyyopq.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gwjuopusa.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/grtxufpby.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gjkaapdqe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gjkwterbd.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gguvltkji.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gdbxouvce.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdtzdhmcb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grtypaexq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ggnfncviy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gbdshkqkt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gzritvsst.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gqpuvmoqx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ggzdlgoiw.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gqwipkrlh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gvutvebdf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gwbafslrc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/grndjofjo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gqwlopujx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gguqznnua.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gkbkpujmu.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gzoeqzzfq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gekohxowk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjanvdgdc.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gblrhxbab.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gizprelvk.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/geesjfzci.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gtxbfzvsu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjgczlujr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gqrurhdrp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gzbbhnmqj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gsonbkjzp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gdgffjpbt.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmztruogk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsudbvshx.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/ggpuqvmvf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gsyahlced.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gnatmnlpn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gzmapoozn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gmezmortu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/grmhycoql.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gjxzeolkj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gartkgidv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/giwjxiagq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gmdgzkpbi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/glpbkudjn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/glywvxkku.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gtiwhlmwi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/grpozitpl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gpytxgtub.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gqdfqttjd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/giplbjsvj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gklwoitsa.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gskmissqq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqniqobtn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gbtzevcuu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gtamyhpay.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gdvkshoia.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gyfqlkxle.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gwbhrarbe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/govtoapby.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gckyndguo.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gqfkzlngb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gwfwmdwww.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gyqapsmwq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghvrcable.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmhlvicyh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gvfmzxvgq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gmfiraymx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjfspyxjz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqoctfmzt.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gmlxqroeb.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggiflrnkr.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gamrlzvkf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmuujzarz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbvkdkwaa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gldydwpfd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtzbwjchi.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxilyvggc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghnijkzgi.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gmogihnsu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gfcajollp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gldznqevd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/ghchcbsko.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gzthheyda.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gpsvulelr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gimnqpxbb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gwefwthwj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gzeyagtek.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gfklqzrku.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/glheijfrb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/geaqefgoy.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gcnjurqbj.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/ggmityzew.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gdddwsptq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/giemwomea.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gksbkpkac.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/ghdraurxu.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gvghuhdld.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/giuojajrv.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxmxyxvnq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gqgforiys.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/givpntfat.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/garrxseol.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gfduipvis.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gywsmmbvm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/goowlwlbx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gbougzqnn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyzavedmn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkjwsixjz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ghotschbb.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gijqszmim.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/ggjfxhywf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtoeoxbcq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggjorxvwj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gotgzjrdh.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/ggujnfohp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfacnnmjk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gkcfwjsyz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gomngtqmr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcshqzxpi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gqpwiyxpm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gnlslsowi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gtbqpmnyg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gjipsalbw.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gtbmetvcf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gslbyimiw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/getvbhmas.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gfktrejah.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gaqgrpidw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gqbsxcsly.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gqxeuumqw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gutvtgmcc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gphzdfjlz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goprwoioc.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gkczorvof.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcorrcszv.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gaosniqmy.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gnsjpvlky.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gmjgzmeii.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmbqhrxnb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/giqnksdpp.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gmhbzzcgj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gzounadnq.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gywhgqzcq.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ggitdtgpj.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gygufftdl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gozxdjpjo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gidglwonj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghjxvfidz.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gypoecfds.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gtsmqcbif.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/grvatvchm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gqktfssch.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gvecnhftg.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/ggrdqnvng.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gaamralad.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gbxhvxxwc.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/ggamxwnfp.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gpfjhvpfr.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gthsgvghj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gvunxhwlf.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gqovhvwvd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gdnnwmlth.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/ggvzadhrl.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gewltowjk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gbfumufcd.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gnqaxiuja.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gwkgjcjpi.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gxwsgtrhm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gpnuwdxed.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gqxshjirk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gmabdfggl.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gckduoxha.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gwvuepiis.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/geagbbocm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gmfzckplz.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjfcywkgz.sHtML


<!-- 参考信息 -->