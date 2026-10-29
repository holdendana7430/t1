代发 wailian999

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/ggqxreqpr.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gfygcyuno.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gcgphaaaa.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gktpykatj.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gyacsylpy.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/genxmyayk.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gqjkbgfnz.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gemdyukqr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gsthdkapg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gwsyzmooo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gwozcotcb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gnrptwhck.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/guzhjwjic.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gojwuradl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/ggpykrijy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gpjxxedqf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gkcarzqcx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/giuylfraa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gktxghznr.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gcquiwlva.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gohqopbch.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gstdrubzw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/grxxkwioi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ggoewigln.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gxudlmaly.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gjypfktwp.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gdlbtcxtf.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gljicbhne.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gczhsgxjd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gzqmgopnc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gawgovytn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gvjmwevzz.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/glhlqnbfu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gkyxsrfuc.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gldgvtiwh.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gikwakyux.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gibdjtlau.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gdarjqiez.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gmzlwdoqo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gguheiafs.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gkguqtton.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gemohctwc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gsjxpunfm.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gjgnetdtp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gejqbgtwf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gfegxmkkp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gkwtezogr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gokyqfkiw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gxlsibgiv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gvpdzgnny.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/grmjnnoqs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/ggdzdnxrf.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gmkkoirzs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gqaeeekau.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gneilrgjz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gmathrldp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gulavupuc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gdielaooj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gxmzmnlzs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gctyrwmwb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gejyouhcn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gbpdzupad.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/glknnigck.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gzowojbvg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gxvadeovu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gzorsutvp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/ghibrkqgu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gdzyynvwd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/glzgdsfjf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtwrvbllt.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gtdnwebga.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/giyxqwkay.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gtnspvkyc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gjijpdkos.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/grcuhdqgw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gzhfwygwy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gewptqqde.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gkfmaofbp.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/grautwfzm.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gcrvjjacx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/grhntuwul.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gvnveucod.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gqbjczxsq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gamagpese.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/givhfoqkx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gojjxqybk.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gnvywqfew.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gqqhkummy.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gvdrncbfy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/glwqsskis.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/groepckxs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gpxfqymea.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gdljvzezz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gzxgqneuz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gvlczadwm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gsbcjdmhc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gbciirqcz.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gujtzcaqi.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gjnyedmtg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gjqwetdtq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gxrcvsomi.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ggvssuwku.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gufbwimsm.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gmpmfbhnb.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gfxccpxjc.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gxafhcwpp.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gnylcmjbr.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gihfsmvrw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gdpqjslle.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/grhxruffn.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gobnpsasc.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gnodzxnmg.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gmnpqgbyf.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gnmutryur.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gmafoadox.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gnzzaxkch.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gtiniqmav.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gbjasbkcg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gifvvvudy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ggpcmchsd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gqvlbkjnk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gtbxqlxrw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gelzckocg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gccbrexwj.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gcjmvlgig.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gwunqtgce.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gqpjifndt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/geaarczzk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gfxdnosvg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gjgnnnnwm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/glpovffkp.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gnspzfbat.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gupakrjiy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbixyuylu.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gfurngday.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmhjjeqex.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gohgrehij.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gizavgpgt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gaihmqoyj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gxnaagzpk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gbpzdegds.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gtpnwskly.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gpaexmyvw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gloowpymx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/giozlhjxo.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gmmmxfvyy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gfhgzwqrp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gwkbblhuz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gggptwzyl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gxfnduhwo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gpluldeqh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gdmnrzwgo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gmqxcgjpk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/ghdiwaphk.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gixrtyzlq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gxiuqvljk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gawadswcg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gmrzukmyu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/glrbeufml.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gatlthezu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gcfeioroc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gpuahjdxy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gxiskuqry.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gjktjigfy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gibjhmnne.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gsqakkdzv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gxsjrfnnr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvqzbuxbt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gogcmxize.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gudoyxnho.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gaukncdio.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gkrqonnhc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/grmnhxhya.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gaqapyhxe.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gktmrpzxw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbctljrn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwciybogy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gcaopfmxh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqequqyc.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxrfghpbh.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnnbaexso.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gsfnairif.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gacczpkvl.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gifuzxotn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gisqiunit.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfqklvscf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/glirjdosc.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzajmpbls.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gswposrpg.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/glisrikbe.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/grthunvkz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gqwvwqiyf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/ghyzuvjgi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/glqajpmrb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gsrbhddsw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gcalricac.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/grqaumngn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/glnyanyhr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gwvnnslzl.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/grgfdnpyt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gapuxjete.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gsphfwwyo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gsvlrbudg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gntpgoudi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gjdvdmtva.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/geagozeza.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gwchkpdna.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gmmtqbnsm.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gxgxukkil.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnqzwojgr.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghetqmgfi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gtftrchul.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gzfplxhkn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gteaxidki.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gipwccori.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdylaracw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/ggpyfbqxa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gqyuzqobg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gitesvddf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqczqkshn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjlfbhmgn.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkhucfvcb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gbzsuefrr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvcfrnwqr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnoafmsza.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsmkzpwiq.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gvzwjmnvc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gqyjwvsku.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gausxllun.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/geyyriodj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gltmlfzhe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gvczupmkv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/ghgysipak.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gvmbgvwqu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/giybsnecs.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gwbltoyqv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gbzmttaqu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/glbwmvubn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/giqdhpuxo.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gopyxdcys.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gdlyupajs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gmknumgfo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gjsaflcjl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/ghvzhesqh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggjkzggvy.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gqtlxjcgb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdfbznnxt.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gwcnqkrcv.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gafshwaes.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gwdxtatbb.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gwnbvucpp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/grvuxngaq.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gcpsmodtb.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gadkndgle.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gmcmlibgv.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ghqwtqpgq.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gxpskuevl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gjcjlgbmw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gcyabtuki.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gnzwvmolm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/glasiiibo.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/getzqlmoc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/grhhptlwm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gmxuqkpqr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkgtoxrn.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gfwyipiqn.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ghhztegpi.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gdmbznrpt.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gylptivhc.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gsfdsykoc.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gseiioczq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gpebmopya.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gheukuztq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gyfvssyxy.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gowxezrsp.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gmfrmepdt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkgaiwvbn.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gfaqxobuy.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gkmjclkzf.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/ggbexpurq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gvtaygvan.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gobkhvuio.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gygsxrumz.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gaoevxwwj.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gbjhkjlnf.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjxhwdtue.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gvdgghpbu.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gywgzhcmd.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gbzvnzxww.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gnfmseceh.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gdwicybgw.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gstwethlh.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gbemdianh.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gulkjepkv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gxxisquui.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gllcmygpg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gmvgkspib.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gsgxsljwb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gkmortsvn.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gamdzlrcr.sHtML


<!-- 参考信息 -->