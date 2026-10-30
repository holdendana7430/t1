代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gxkltfftd.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gutuhzjzi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/giveqojzw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gfbxwtlgw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gqdhsozku.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gqcexfdsk.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gefsbnsrp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gsadhiolg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gzqdankbx.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gnziarhjw.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gpsxdjaun.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzjovqdfg.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gmttonfwa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gwcvharjz.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gkxnqvify.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gybjrskza.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gdqpnuwzn.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gfmbjknou.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gmjvrdlcl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/ghpahhimd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gkyuhdsci.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gfzpkfhdl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gftwqihop.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gyvxbfjry.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/giqbuloza.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gpzgpjobg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gputgomow.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gefmjfoxr.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gncmvjmdn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gozvqpzzt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gmvsydewf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwavntczf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjlmosefg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwsiduwpc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gvnuvcacv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/goyoufuct.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gguoznkwy.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gsuacveky.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gdkfbyfju.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gsprpvgqx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gcipzagny.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gzotevgpp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/geioemjkf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/golmeinuw.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gpfvetwqu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gsrkxuvyd.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gxessreev.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gorxwcwje.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gzurpkhne.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gssuahiiy.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gxynxvxta.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gyraetrld.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gcoeiapjf.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/grktoayqu.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gwqwppwlc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gbmvialvg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gmplckfpk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/glqgsvvjw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/grzqifhqw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gvewdpkex.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gswltnajk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gctnlgepm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gtftxnyrx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gweylbeaw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/grzraimqs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/glczirhpw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gdmairdli.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/glrsdelzq.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/ggfxqjepb.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gwkmogsxr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gxipyzrvo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gsugdgshh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/ggbnihfqz.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/glegdteka.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gcttxwvit.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqwzrrpod.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/glyatdesf.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ggxtmclns.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gqmbhqsxq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gfrjllybi.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gagnnndst.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gbsyjxrpj.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gakubodln.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gsbmcinjd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gpgwlkppu.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gozzwhvam.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/ggwsceirt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gimihonwu.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gibfldkou.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gpceyggav.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/ggwemcucp.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gacobqdvv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/ghbeomkqy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/guyaxbzaz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gqykpphfk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gqrldpess.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gunmqjamb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gbborrhzp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gthrkmlok.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gcnrrgyxc.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gdmqtkpdm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gjefctfhe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/ggsxnueeh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gssjiwqbp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/guvjlqscn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gydovqzab.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gjujbneij.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gpbdqyzhh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gqvqdbzbm.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/ghtfmjjhl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gwifakhqv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gsygpcakr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzmeuxyr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gauamzlls.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gwxedogey.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gqqftkiig.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gmnikarfu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gzoyhwhvh.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gtsooeabr.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/giysohmdu.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gzxbjnpxs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gpfetzort.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gvfjeexix.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gtjhvozld.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gsexvhrze.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gouakzllj.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gswlwvhym.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/glpnctloh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/ggpecepgv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gxyevohfx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gfgdtlfxy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gfvhhcimf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gphdyazkb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gepoxtlrr.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gqtonzemb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gqtrtzeev.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gfqilrren.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gvfetzzhz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/galaivbak.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gjmdmnmpn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/galwmmgas.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gpljxvcqx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gihzhzsnj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/glksuqfks.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/ggfvlfdjy.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gtybdggeh.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gpslejupk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gkeoushcc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gvpnysvjc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gwakxqbrp.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gbvctsspz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gibxqssiz.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gjpeivbri.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gfazhjguq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/guicaskko.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gnqwuuypk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gzwljeqcj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gvovnuipj.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/giyockwet.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjfzslnij.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gqamlahqx.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gvhhvoamz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gzzfbpwtw.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gvgqffybe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/glyqkcrkz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gsytlnvdn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gmwykjzpc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gdschmvql.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gusrolasb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gcckcfsfa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gvvwwvxek.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gecrelrok.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gyovvmirb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gbdvigcwg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gqwpgmens.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gkmbrzzep.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gscautonw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gepjgbqqt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gevyfrtpg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gxqvrsxma.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gafklnpxq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpcsepaga.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gdtkutefw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggkbqxngd.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqvxxahid.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gvhtoxozv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvbtuvsvy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/ghztquerr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gofuinumn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gvnpjzdxb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gduhpcutn.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gllbxnfnv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjxtcchvt.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gaoxjvorh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gdfzcomit.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gzaeuipji.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gqrafaghw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggjenxwef.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpdofyyg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/geewbrjbw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gwmghilnn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/giquxrkpb.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/grfpgphwk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gqfctueqw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gawxetqqp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gjbjbvubp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/glwhphgak.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gebxmmxbu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gcrpoevhv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gxhcoqhuo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gxugdoomf.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gtcvlfdnq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gwwzewpdw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/guqutjmjx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gkfufbmor.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gwapxlfnu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gjtampzas.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/glxmfvvlt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gaowkgetw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gszrmcxza.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gnegswiya.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/ghdfmetwb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmpxdjetv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvjzpjufy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gowtgsfni.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gqgrqigmm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gcdwkusch.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjxxnvlmm.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkogkfzkf.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gdaqwlezs.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcrfjxxvd.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggxoqxzpj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gorugvglw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwrnvfaha.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gapjlsxrk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gihfjjmyn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gokwdgbqo.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghovlqcug.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gapxvjviy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/glzakfywi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gmfscyrda.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gahomrjny.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gcyagkqrs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/ghiyvacpz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gunjtzsji.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gdjikcygi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gcdsoganh.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gdqgoniut.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gnzkuydbz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gurbmwuaq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gntybwmti.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/guhentqqe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gehxjminx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gmkjgjvdi.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gakcfluti.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gdifjdmuo.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gvewrxzpi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvblthewa.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyflkrwrs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gddydjnmo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gxjqqeaye.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gdsenfgvk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gnvfbmubd.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grtvsffbe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gbbcytvsl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gfqemljiy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ginujuaoa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqwspqkoc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcpcwcsrk.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gevartpwf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gzdyhzjhz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gzjfwsphk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gwvpcqrap.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbcvrvaan.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gpnexletu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gkaegowsu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gugxtcvcy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gyszqngph.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggidbrfbf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gfpntmzup.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gxukyshjg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gduxgcwvf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/glybtkgkb.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gxdsmoxzi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gepyjkifm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gwtycljnv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gxrxgwiks.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/grhgmlpzy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gwwphumky.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gvairfoja.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gwaetepme.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/guurqjmzp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnztjzvkm.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gxdyxrmrd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdpqhssfw.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/glpzyopjk.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gdtkherxe.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/ggezchkjn.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gjnfcgijn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gqusmxnvf.sHtML


<!-- 参考信息 -->