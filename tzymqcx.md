代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoaitzso.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgbrhiet.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glogouakc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvrdwiqk.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiobzumg.sHtML

[E07] 按分隔符拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gqelfkqlm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fanxiaobao.xyz/Article/details/gshdxfxzm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/glaedrkzg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/glckangxz.sHtML

TS:   s.split(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmayeclq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fanxiaobao.xyz/Article/details/gtcumubnh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gujmunter.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/guatpling.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoypoijp.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqppmaqh.sHtML

Py:   ",".join(items)
来源：http://baike.fanxiaobao.xyz/Article/details/ghnbltdqt.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcdpkooy.sHtML

JS:   items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gglbvioky.sHtML

TS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmniqbzsz.sHtML

Java: String.join(",", items)
来源：http://blog.fanxiaobao.xyz/Article/details/gmrtpjnep.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fanxiaobao.xyz/Article/details/gdecpojpu.sHtML

Ruby: items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/ghqkmeltc.sHtML

C#:   string.Join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gcqphwzcj.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfbhnbrm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwreguzb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gnjarshto.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurnagozz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gdhydhnmx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdlpiprr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fanxiaobao.xyz/Article/details/gqpvtoade.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpdycpou.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhtqnjhi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvdxlhvw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gqlbxzxok.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fanxiaobao.xyz/Article/details/guwlbmnyu.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcarymop.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gnbzbvbyb.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gxaevfrbu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrfyobko.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gsywxhusz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grchtuozo.sHtML

[E11] 反转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtypgmkq.sHtML

Py:   s[::-1]
来源：http://wap.fanxiaobao.xyz/Article/details/gvtgaurbo.sHtML

PHP:  strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyvnmkpx.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxvxjail.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gonehmcmp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gyfutfivc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gvaflgrqr.sHtML

Ruby: s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmjyktsr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtaecqsz.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfsrlntc.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiznqyet.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fanxiaobao.xyz/Article/details/gsopwbuyd.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gnzqgfkfx.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/ggkffzdyp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpmiyjjb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluusygsq.sHtML

Ruby: s.count("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxwmhdwb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fanxiaobao.xyz/Article/details/gwkvkiznn.sHtML

[E13] 逐字符遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwecxwmyj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzsqcimj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsuaktzx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggugfzxqm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsogmplwh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdympuicr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gpineqgqx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fanxiaobao.xyz/Article/details/gmkdyakac.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebkvjyzv.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fanxiaobao.xyz/Article/details/glsrmjdxj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fanxiaobao.xyz/Article/details/grrzzgcfb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gncpvblmp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/gssmzyfub.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjyggkrf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkakqqls.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fanxiaobao.xyz/Article/details/gyiasrdzs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fanxiaobao.xyz/Article/details/gqmsolimh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gkclddikp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpmxesrs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/glryszuzg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumuazjdc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsyogpho.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjirflzh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fanxiaobao.xyz/Article/details/glrkrbfyt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxhpbgyg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmtufmnu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjgtkhzce.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/ghoskggou.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtljryjdy.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiudmqba.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpptzubeu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fanxiaobao.xyz/Article/details/gtoiwnmnp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/ggqdzkssf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fanxiaobao.xyz/Article/details/ghxedutmm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gqvpoczle.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfffdnbja.sHtML

[E17] 首字母大写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglqxgwci.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guviihhrw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffgqhrwp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdkibjak.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyvyvgtj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnoliieft.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gatziwdyb.sHtML

Ruby: s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiychxjz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fanxiaobao.xyz/Article/details/gwemzcslc.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyyrlsgj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsappafzc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fanxiaobao.xyz/Article/details/giauvcjew.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfaztabh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgrzhcqp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbzyzedr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gkznifnfe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzdzeopg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gksbgwquq.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzstkzxkr.sHtML

Py:   s.splitlines()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwzlcrje.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstsmvczo.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fanxiaobao.xyz/Article/details/gsfrbvdgb.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/geydcgehy.sHtML

Java: s.lines().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdavajwt.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gogarcknl.sHtML

Ruby: s.lines
来源：http://read.share.fanxiaobao.xyz/Article/details/glqwzrsoc.sHtML

C#:   s.Split('\n')
来源：http://wap.fanxiaobao.xyz/Article/details/gajvqpskq.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fanxiaobao.xyz/Article/details/gzklzzayz.sHtML

Py:   if not s:
来源：http://blog.fanxiaobao.xyz/Article/details/gffajggyr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fanxiaobao.xyz/Article/details/giwxnmvwi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbivrxupd.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfimyegsq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvaptcbg.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwhapeze.sHtML

Ruby: if s.empty?
来源：http://mobile.fanxiaobao.xyz/Article/details/gqambeygw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmzddrkce.sHtML

[E21] 超长截断加省略号
来源：http://baike.fanxiaobao.xyz/Article/details/ggabkozaq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzewskogg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/glnyxedqn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgurocaq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcsufpmp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gzdeakyun.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fanxiaobao.xyz/Article/details/gpyhmjmug.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gnicbywfc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gxmboxzkr.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gprnmoqqw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgcliehl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmqwqwpf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gewamnhar.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkocbbvze.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gefxefdwm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fanxiaobao.xyz/Article/details/gwhrchpou.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzynfgeo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjeagxah.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdgecyrp.sHtML

F. 文件与目录
来源：http://3g.fanxiaobao.xyz/Article/details/gakwjlxue.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwnsrgjih.sHtML

[F01] 读取整个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gagvrrjxd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fanxiaobao.xyz/Article/details/guedtejso.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gmzplrdxw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fanxiaobao.xyz/Article/details/gwknhkxyz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gllnfmwep.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkcfcksq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrvsldyt.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/goawffvcw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqqswsuy.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaurriejg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fanxiaobao.xyz/Article/details/gxfolyhxz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grsognetf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxzxtftbh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyocdbzz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbqidxxb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gursfybgz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fanxiaobao.xyz/Article/details/gpawyokje.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfftzrhzw.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fanxiaobao.xyz/Article/details/gfwecqkvk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjonojtng.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gqvxcjexw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkanclnhd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gngbbyrxh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/ghdxwoucv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgvvnmqg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfhmdvql.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyhfnhya.sHtML

[F04] 追加写入文件
来源：http://blog.fanxiaobao.xyz/Article/details/godljcluj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcuqcabb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fanxiaobao.xyz/Article/details/gnwzpbpej.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdykdfrrq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gpaptgoqg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyczeqiit.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gdgupybzm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fanxiaobao.xyz/Article/details/grpnpcemw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fanxiaobao.xyz/Article/details/grzatxdks.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/geiapekfl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fanxiaobao.xyz/Article/details/gxwumrwgu.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gayfsbwjc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvefhfisb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggheqehjr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynwrldfo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtufbgxu.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gzolzmahx.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gspkqpbhl.sHtML

[F06] 删除文件
来源：http://m.share.fanxiaobao.xyz/Article/details/golqfgpmf.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ghxillami.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gmrnquhry.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxaeywdq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gzwijjajt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gkmawrrco.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gtmoxcqwk.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gdusyknqi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwbvtnxl.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjuomwoa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gplpssihy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gyrvygjrm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/gwuercyom.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/gntpecjuj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gskrzluhw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdqkvgma.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoaaocjt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbjuqxut.sHtML

[F08] 遍历目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykvenalz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gqebxfdyq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fanxiaobao.xyz/Article/details/grmspeerc.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gumhgifdx.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/glhmntegr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fanxiaobao.xyz/Article/details/gedtulhcb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/goqktyulw.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxutfnhu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnicdjxip.sHtML

[F09] 获取文件大小
来源：http://blog.fanxiaobao.xyz/Article/details/gvclsjcvg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/grbnslaks.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejtrwanz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/guowvbztb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gpabxptfo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gkivbaovp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdpctfei.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gciylgghn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gxktmllwl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpsugxer.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gmdleonoc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvblfvrpd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gobvvdsem.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gmxrsenaz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fanxiaobao.xyz/Article/details/gqlttggqh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ghgztfnml.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzkwhzes.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/glwzbajav.sHtML

[F11] 复制与移动文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxuncqxi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/glfviqvat.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgmrwonm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gusckxuje.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gxsdiigwo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzzewokj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqrrfrzl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gipsfwvql.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprjgiuub.sHtML

[F12] CSV 读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrmwgrea.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfokbkuay.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuexxzdr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gilykbfja.sHtML

TS:   // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gagmoxidj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fanxiaobao.xyz/Article/details/gzqubswiz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gspwzxchm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtqhsqdg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgbjrmmr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/giqvwboce.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/gzacvnvko.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlcfarbh.sHtML

[G01] 定义类
来源：http://read.share.fanxiaobao.xyz/Article/details/gmglknsjm.sHtML

Py:   class User: pass
来源：http://blog.fanxiaobao.xyz/Article/details/glejvlhst.sHtML

PHP:  class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gevugrlrd.sHtML

JS:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkhycjnc.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfucfjuy.sHtML

Java: class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrrczseu.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvczcfeb.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/ginhazlbm.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzrwwxrde.sHtML

[G02] 构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfizympe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiqklffs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeaunvgr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqirzvjio.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoyqtymp.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmepznkil.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtamazhsf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvmoqhya.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgndtwlh.sHtML

[G03] 实例属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysioxpzb.sHtML

Py:   self.name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjljdylkt.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzbrraju.sHtML

JS:   this.name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdjottqn.sHtML

TS:   name: string = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgesdsec.sHtML

Java: private String name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvnghjwk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fanxiaobao.xyz/Article/details/gunknctac.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnvewjbt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkwebamg.sHtML

[G04] 定义方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhpcguyc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlczselz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzteeomib.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtkosmfv.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcowuncjf.sHtML

Java: String greet() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gktcgfsnm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gvzutebff.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkptmqlj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/glohafsvy.sHtML

[G05] 继承
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbckbphc.sHtML


<!-- 参考信息 -->