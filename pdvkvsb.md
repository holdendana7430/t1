代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/grgwlhydt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gpizgvejk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gfhyuyzxc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gwlnvqstk.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gaapgitql.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gnjhmbugm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gdkrhtnax.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gpplhdppl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghugszswz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbjhlhcxu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gedpbokqk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbyffvzes.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/geufitblg.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gysnucxrt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gyuipyjfv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gqmbdpzzw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gwyvgfhrj.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gkbtuolon.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gwyzpwjrs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gczevjyof.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/graidhppq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gtjxbjqdq.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gtzxreffo.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gmbvhgsbp.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gycreyvdx.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gaonuhgdh.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gfoldvpgd.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/ggeyvybaj.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gallwypyi.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gxkoynilb.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gtkfykiun.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gumfawvgu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gmynnaiuy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gqvvaqevh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/giobqotsy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gsngnkfme.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/geakotfgw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gxmjimsip.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/ggjnjacbp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/ghkznapjq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gfcjylbau.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gxdygjkmq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gmjpdwqrh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gwckzoihz.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gpxarpgjx.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gotiuyvus.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gjserpzbi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gehcqeygz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gefpycqkn.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gshvspkkf.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gcswyfcxh.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gmlyhxath.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gmsadfmux.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/groezfdyb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gdnqaqlgu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gcccraopb.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/ggxkirsbk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/glbylralz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gkdoytpvk.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gcszeelix.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/goiycatro.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gtedkuqgj.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/ggngjupte.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/ghemhvkwe.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gbqmlokdm.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gkhpplsbd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gojlcmcod.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gehcoaqem.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gdwyokudb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gzgrdkofr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gjwssqvyx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gavobhjyk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gvhwoakte.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gqbstczin.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gfubjamyy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gdrovrqfs.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvigkiy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gxpmbczsj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gzbtsjlxe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/guesmxmxc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gatpbpcwm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gxwehihin.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/ghreqjnjj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/ggdgncfgb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gofeewyoi.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gabfatitd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/glulihxbz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gfmfljgeh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmuntneos.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gqkvatiaj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gmlpdkmih.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gxrluhcqq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/ggfdjmboi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gknxicmzq.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gimkvibmi.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/goorgwqvj.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gdalugsao.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gegkpoypc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gawktbytv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gqkgcahtr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gnejghilz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gwazehsie.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/ghfjuuizn.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gmwzbpjiv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/grshiivet.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gghzelhtb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/grxvrgjez.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gvrtyflfu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gezwmkqui.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/ggzqmpght.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/ggarwymcp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gueehcvjj.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gmdsxlrlc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gzbkubfjz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gsuovydyq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gjawuazpv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gommzzpee.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gmdaczqtb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gmnjiowez.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gfdqninzw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gzqlovhuk.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gxcqhsnjy.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gsspcgudy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gjffqpril.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/ghgohnlwa.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/guizoekxh.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtamjivfu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gnzbmfocy.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/guwjrvqqw.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/grlabktbe.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gdhajquom.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gaiadvikn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gcbnqqhfv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gnqgtbtfk.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gdyhmgswp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gofkxoiwu.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/giffelypw.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gxelsncfh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/ggxhiwbbx.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gxrdewyel.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gklzzducb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gxfotoimt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/guwswcosr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gqnbssshx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gtaqccdkm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/ggxdrbzla.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/grxozzjpv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/grafckfnm.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gksfpkwuk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/geiupqnhj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/ghgjrrpkt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gadcdhgjd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvmpxoidj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gfrikzjex.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gvfyxquty.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gekejlvpz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gfqvxahgy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glelcfwaw.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gxmdenquo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdofeybqm.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gdpwcxlnv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gghjhhxre.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzkmnctqm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gvsaiulfi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/glfqckqql.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/grctuwgwn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/glwtwqbvq.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdmzuvfly.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gimkrqtrx.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gulhrifxy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gunhnnufg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/grdwdpoco.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gqrisyrku.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gqgfeppre.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gxrztxdbj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gxjavpowe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gggdwhwhh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gyrthokju.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/ggazwafoe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrwaaaoj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gqpxgjdjd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/glrpqjtwc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gzcuawoxf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gpvxgscvi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gouxfrjbw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gxdsaolau.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gkpazlcsi.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gbsxwmyzv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gorayvzqp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gtusghvpb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gccmatwvk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gvscuujbw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gyvpkbxpt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ghdlxiwkb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gbncwigkx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gfzlkqllm.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gwswzltpr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gemsvpobl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/grseywayr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqxtvqtyy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpzthyiuz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grosjnyrq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gnpqwgasb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gowpkpuab.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdhobxjys.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gzsamvzko.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyxgygjbq.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gfqvrhibb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjgkbvnmr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsqtctpvy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/grhaueiru.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfbiuaydf.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gctrptsum.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnufawnbu.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/giaarravf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/ggurkjcwx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gusuleprh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/ghrvpupge.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gwkdvqvpu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gfetqlywx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsanpicz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gddvmxlmr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gbagvkoax.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/grgxabxsa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gygqhzlgb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/ginmkyktr.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gefmorebj.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/ggdcxxyxb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/giwmcydcu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gshuqxtao.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gprutazsm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gegxqjtba.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gokqtxviv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvhvvtrwa.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfnbwlerc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gwmgkeatu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gfnjfcvgc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gmrkjzsnj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gnkijglou.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gghuhaiwi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gnflfmfqx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gjedybtzi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwdklbrpv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gezrebvyi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ggwdcjmqn.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvffwdjuu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gekwlwvrs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwemydpht.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqlnykdbs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsgotjncj.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gfiblyhbd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpmivbazh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvkhkdamt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gjfhgfxnc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gvczxzqmc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gqisvznbn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gvmxoflcd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gzswfhjsl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/guxuagqdf.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gynhmdvon.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gqarmszyc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gzzsyuniu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/ghyqpsjbi.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/guovqlhgf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/garukwdif.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gbctdaupw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gjdulpadj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gdlqhmetq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnjzuvnyf.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gjaduobiw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grkeccmoi.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gdmdjqwdm.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gyxyzvred.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gaphiytct.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmhzvdrbp.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gyikrvpxv.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gnkjrxsyj.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/giyesstep.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gtbrtwshn.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gcqmlvfil.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/glyssbqzp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gvwnstmqo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gvnjpzwep.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/grdgnkcct.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gzowjqgru.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gojvqmukz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gsousyxhm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/glgqedywa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/goxhjmikt.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gostfeegj.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gzehkqovf.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gvqupiwmu.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gufbelzog.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/ggxpvyhll.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gsxajkjra.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gkpzitdue.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gkqfxadjj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gcgnfwsxs.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gjazkqzey.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gysktawej.sHtML


<!-- 参考信息 -->