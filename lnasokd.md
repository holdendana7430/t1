代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/grvhphfvd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gluokfrgx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gjcpllyoj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gcrwmhfym.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqzbthpfb.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gznrfglvo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gfcmkcgnp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwbrcnrnz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gmtilpjhi.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gknqjzvwn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gmkahkfqc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gwnqhndvh.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gwqljwhhy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/ggqrlpxjp.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/geoefrqdp.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gekedjatu.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gzxfuyqth.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gsjslveam.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/goewhwvpr.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/guzcotkip.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gztapsnww.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gvhcbluhd.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gspcojfmn.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gmrcjdiue.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gtvyykvjm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gyiptqztj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gxofzfmvu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gpxensmvw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gnsvdhmqc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gpvvgshld.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gktngaiek.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gneenvdrq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gvwhedtfm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gjazquvvw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gmvktrlxq.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gubtfegwi.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gudetkodh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gpgsnrjfo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gdlrkkkfc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gohtkqpwb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gaomggnyg.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gxtrfapfi.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/grxiyajaz.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggzrwsdem.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/glosvakmb.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gsalumvxq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/ggnldzpah.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gqpruqbmd.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gwpmyyrzm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gazfmlybb.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/giarsgqls.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/ghbznsahu.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gdzcocava.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/ghhntsobb.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gqqwzvkol.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gfotjgipy.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gihcszouv.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gokxfvwdl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gjxjfdgbr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/ggekbgxbx.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gvvlgsicj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gfzibepat.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/grlzffcww.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gfvxawvmr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/grgdybdpj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gqbgbvhth.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gwhbpqray.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkytcohid.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gcthbfmjj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gcvkvuhfl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/grdsrwasv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gajdtuesj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gklqgwwmu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gowzcyzet.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gkaodacnv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gqhgsaitz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gwhrxumbx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gdfjsapsb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glzdcgqwu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gosteloif.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gupkqlhzu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gdmtxqxbn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gvqvimlgi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gtvigwtsz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goobsdrun.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gainokkrn.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/galfazdzt.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gmuajwxbk.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/guhthxslm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/ghkuznizm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gllmltpad.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gclnflqro.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gcjzcmsmf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gnvfdpetd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/glizrqrma.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gtngdypqb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gkrhbevud.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gokawxumy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gxygpnexk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gridjutap.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gqxkywzzn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/glzktlipp.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/geieeprss.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gqudbtxqi.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gcgjkmxpm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gruqooyxb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gfuazrcah.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gbynidwhl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gorfxdrsw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gzyfpvaoo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/giwpqeewx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gjanaoxhj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/glfopszfw.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gdvhlrynk.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gpgudemal.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzbmwdrne.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gnzmdycbx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gmkwkuylb.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gsyqgnovd.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gbsoxduuy.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gapbjcivh.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gwwsieblc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gnlmokhlu.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gwwjkhicq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gvobexcnb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gxpsxbczc.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gliwezawo.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gxtfghxge.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gmjrykjsa.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gbcxcgcqq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gmhfqphlp.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gaqcscmkp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/ghlfrhchb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gpvkokxrl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gjszghjqq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gnlvqmzew.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gblhjupqy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gzhiymcov.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gxjmxzfsp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gvszknqlc.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/ggfedzywt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghzvxlwmp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gnrncigbc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/goaoxjexn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gophusvxh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gpezqkejd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gyzrqcisg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gfwnvngsg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gdfxdbsaw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glfaurthi.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/guqdhswcx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsmekpspq.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gkjrrnvbi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gqslclyni.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/goxhobsuk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gehmkiiel.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/ghwwfuqev.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/geutkjife.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gdelyasmt.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goowgwkou.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gidomgxqs.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gjdfxpsvh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gydqrpdne.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gzdnycrmb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gihtolbiw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/ghmrhkjox.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/ghdstzifx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gnmnutyde.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gwoixgnxo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gdqdfrszh.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gfhhxpdso.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/ggntfcsud.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gzyvlhspf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gekeaiqyy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gbesjxzly.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gblnkvsaj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/grzqtajvy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/ghmxnonmg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gairexaha.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gbgrmjeuo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gbhndwjrh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gzeqrinhv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/guszdxeim.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/goejpprks.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gvekcfbnm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gkplmeozm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/guvloqtpz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gckjmpuvn.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gjyqmnuku.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/guakbfmvw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/geedmwvey.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gviacpwag.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzduczbvr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gvurhxagf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gjhfwgmin.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gakwfpvpk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnsgbyfwg.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghokpzbpb.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grsotainu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gomgntbnd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glksfxkzy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkwfvvobx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gzaihauyh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvrptfehk.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/garatnskn.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqaffrnpr.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/glbutqchu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gieiofxwb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gzhendecv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ggxutmbdb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gywdcuswi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gndxbizvu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gfnemtmqo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gillvqrau.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gyadfmoir.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gksukyeok.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gafwnoxlj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gkrdkqvhi.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/grwwapwaz.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/ggqmboveu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gohydagoj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gpmjvrasr.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/ggzejqqvt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gwgetwrcb.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/ggtdszxgj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbssdipor.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guqsqmthm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gcjnrcnqc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/geaclnyza.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gkurlwrct.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/guglgprdc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzmnyxsab.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/glqhgkqdm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gosbycfom.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gitlqomtx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gcujoyhml.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvyqptvpg.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gttucebid.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gjjuhvazy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gosbhjilc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/geabfefju.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdkrsihjc.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gboywbbkt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/groqwobgy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/grkwrxdau.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gxyyglfgj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gerpwqvgc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gsauqnkcg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gmwwulynd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gfqswizsb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gxvothevp.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/guhtrdtwo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gsjzowxcb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gcmmabjhi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/guxmhjxti.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gcndxnvns.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gflbdoxhi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gzwkiqadz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gmpoeerys.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gqinjtiqp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtliakyve.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/glnczkxbg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghvzorwav.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gelfkvmth.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gxegagnak.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/guklpxymm.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gvsyulwto.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gvhiylpor.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/ghnkxyivf.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/ggrhzhykk.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gjfsooqqr.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/giinxolji.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gzmiuxwhg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/grhmxpfuj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gbikmkpja.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/grspfqufk.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gmpjubilp.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gacrtgcqp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gvlhissfi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gwvhfvicl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gqadqqvny.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gfeeranxs.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gjtjvaqgm.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gusejywhj.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gxulrwdys.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gjxgxruma.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gsekfbeko.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gbtntyfkl.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gqzxqkpaz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gkbrjskuc.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gmvhvjtzd.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/ghxevhakz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/grgdlfoog.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gfksjfwby.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gsyfsogjj.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbaocbixd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gmdcxbemr.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbudimxzx.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gzohuxwry.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/ggotjhdgc.sHtML


<!-- 参考信息 -->