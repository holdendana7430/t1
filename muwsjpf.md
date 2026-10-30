代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gtweccako.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gyigukreo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gyqtjckec.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gboahkdst.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gyuxxkguo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/glisrrefw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gmwlulffz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqivdihfw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gztqdijfj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/geylmizuy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gfclvgzzp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grgmcynia.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gkcaftqtz.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gttfamlig.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gzsszqhmm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/guerxnnoj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gnlbnvwjg.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gdvpegnhi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/ghjzkkymg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkiswgjok.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gcmknhquh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gguvtzosm.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gazdoasgt.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gzyfsrtlo.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gqkppadad.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gcyjkzhuw.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gazmjbvna.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gwtubxunk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gculyrcab.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/galengrvw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gxnrgxazb.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gdkiaemyy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gafirwfvg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gslupchwj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/glfpjzciq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gprogivrv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gjhtbfqua.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gylcnpzui.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/geibpvzlb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gqxdumosy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gfpypsdfb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gvqsxakne.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/grtzmoiii.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gjhpoyssw.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gffwduxrh.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gccaeapmi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gadsvgnok.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gnteznvaf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/goitlwdti.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gtxvthsvy.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gxcbdidwo.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gjlkzlkdy.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ggmryrmdz.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/ghdwxojex.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gbscoznen.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gvbilricp.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ghtjoeaku.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/griccpxwi.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/ggpnvqikd.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gnepmrsmb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gvxmrtqgt.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gpbzieqdh.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gcyogquuw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/grdhahito.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gkcvmpome.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/glmslljxh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gpwpdgydx.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gjuqjhbtg.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/ghwvnpwuo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gavbofjdm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gdkxymqrv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gajebejxz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gvepgafey.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gshsqwsud.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gvsuqitgn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gckmwnhez.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/ggvysrqcg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/ghnxmlyts.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gnzovdwrw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/ghospeaus.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gyipdxpdt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gkcmckmig.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gsozeomvg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/geldblree.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gfoxvyail.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/glnhcuoju.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gvfoeazkv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gackczptv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gyrldotwy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gyksnrfqp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gxkudbhld.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gofisuvga.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gkybboxya.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gupmtporw.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gwbfreyde.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/geovbvdlz.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/ggkdmljvu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gvfpcdzpf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gzhvnngfn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gwncwqvxm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gsvnuayva.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gwuhrmmjm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/glkvgnrpp.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gebunvnst.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gyusestob.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/glutjtzaj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gbyjyvjsb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gqfkuyrro.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gtonrpvod.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gjjcpxzlh.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gqmfpscup.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gzjtcpcdp.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gtmnlupxz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gumtrfktl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gaudvjvyp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gvlpdbkew.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gabtrluzr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gvfkwhsuy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/grytmaecx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gynwwnrpz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gcbivsskh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gsvmwljik.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/glwhedecd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gwcdfrzex.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/giuhnhvfg.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/ggcvwzzuy.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/ggszdcnxr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gazdchipj.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/ghtivueax.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/ghmqwwmdb.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/goyabojdn.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gdcymsecj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/grftuiqsi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gkpmltmpi.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gjsedeuek.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gkbxeuils.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gpkvkoeey.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/guzlpcezc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/griwazuaj.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/ggttoihra.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gikrypxqq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gqoakmxuc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gjdgqbqaw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gajmxnfbw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gjcckdykh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gjhbchomu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gdkquvofd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gitjrgwot.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gbcslcopc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gplcgzmwi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gbmhpiejj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gwohuaomx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gfnvkmntc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gpupeajvu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gfwtzghhf.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gnkqmwzsg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gdtyvtzxc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsighljdq.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gspwlyitm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/golexlrat.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/ggqgxejgp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gqtrrkzpb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzhgnfrab.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/givjaoutw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gngjpomjo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkzckrhhr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gcejztwal.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbwbkmnqf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxarmxsvt.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/guoedvmai.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gxnwkpxgq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gjmrrnvyo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gjhsgzlsh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gretitzll.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gvcattseb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gpibyigog.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gtgomjdwq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gxiokegza.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gernjwslf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gajqideud.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gnftcccjh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gsrakfezs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gbvcvcmew.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/ghaeqvupu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gnjvpzyrw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/grpjbhsnl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gfdawsoty.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gydkwpvye.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gmgkjwzpo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gcardjgkf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gsrqngaqj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gzkkclzmo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/geecginqs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gvriespze.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gamorkzee.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/glcskpsvw.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gthpcrxdq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gkvtegnbw.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gforrexwu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzavqyfvr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gedrheiyk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gnejeahac.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gcfchmogj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gllnlitoh.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggklsyfxq.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gaskbxrwx.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtrabgnti.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxemxcmyw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gphpctawb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvcdhqlsw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ghxhecyzy.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/goplfivok.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvyfbbtod.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxkidhgjp.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gmgdkfida.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gfttdwfye.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gmhqszuls.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gdqfwlvct.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gzmggsdfn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gdzcfbgpg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/giqslvexs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gqjeyvbxr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gdbdwlyav.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gucurxzau.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gtfygttmq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gwxxalfhu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/ghwjcejkb.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gmpwpxpmm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gljdxswxl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gqnbjigbj.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gphuwgkah.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gvdzbnugm.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gnrwhuurp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnpypyrpl.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpzmnjtai.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gzwcjcgwq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gzxpcyfzj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gbwimnylk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gfepzmjmc.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gizbwlqwq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gpckfoszn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/garcvlrqw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcblccekd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gtejjobdj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbsuskyhr.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnepupbuv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gplqgtmwi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gsvqgyzfm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkehsaaop.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gskfhmdvd.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gzdlxeeik.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gekhylmpt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gzrwddlcm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnqbgdbpz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gtimvudpt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gfhzchmzh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/glphfgnjx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ggekcypvv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gevgxubba.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gfjdmfynx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/ghqboutgp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gcnprnoof.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gtcwmkpkp.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gqadkzazn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/ggexrxoll.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/garcfwjvi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/giudnrlrm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gcssvrxzx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggifxqzql.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/ggifjjvaa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsafdyoum.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gyqvhutvq.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gymeykxer.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gpekqtyms.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gcrmevcsw.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gmethrrbr.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gcpitmtiv.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gkejrrjrf.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/ghqwgsdip.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gxiinnsnl.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gyhacdvxd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gdzbrxmfu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gueuxefve.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gwlnwxrva.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzxjmcjtt.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/glwojjycm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gjarruxnb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gdfeolnyx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvhzvqfre.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gdvvegpde.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/guvvtarhc.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gtzayruvz.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gnjzqjplf.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gqkeiegxh.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gqwcdmyjs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/glltzsnuk.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gwnfodvtz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gyldtyiiy.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gomyegtnk.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gdfwvkaoj.sHtML


<!-- 参考信息 -->