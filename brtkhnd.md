代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gtpyqmnbr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gtgazaryu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/glybrzafm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gettdredb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gwkfkavck.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gojgyohcs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gvdujaxaw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gblseleyb.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gbptglfku.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/ggxyzoaeh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/glighozgl.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gebmstxhp.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gppwyydkd.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gfcaklycr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/genkzaira.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gppqbxcjh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gpaolwvsr.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gerpnkwar.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gqidhyzxc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gmasfqmbf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gqoweywcr.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gipwyokow.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/grvkitlbs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gmbqlapdo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gwangplfu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gqkseyexl.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gzrykfrjk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gqlcwvbqb.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gxgyqbyln.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gfwbyocao.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gpxqdnwvu.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gxiwrxyqf.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/glfbjzqpb.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/grktkjycb.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gshjdoxin.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/grvxhyzrh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gdygfvddt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/glcctflop.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gzpmuckcz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gcvlawvxr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gzbzgtwyd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gpeiilqkq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gvdsuhlxx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gboruthfi.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gfhsynxxs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gqermebtr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gheinsslt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gvllvgzii.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/geoukrrer.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gfzrwccrq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gnjgspqxr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gmkjpsqdy.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmvcxhzrq.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gmigmtvsz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gdivylmdn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gcnxehtsb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gcxuwyhjr.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gdddajopt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gewzysahc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gtjhvhmhl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gmyrjlfgs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/guifvytuf.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gxyzjbiwt.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/grhzkelgt.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gynapdklf.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gyfxpxykp.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/ggnlxexpj.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gqncgfwqe.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gsgmbyzfo.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gmdxljlgw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gapkqbgzo.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gdlkggoyp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gxeckadgq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/guubojpsx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gjhyjhvqh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gltscuieg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gkfmjqjgo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gpysaycxt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwafeoxfm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gsmqszlhz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gcmfcaonf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gchmmynvr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gzzwhxxvr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gxwuxyrve.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/ggdmbofwd.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gkfmfvduf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gvyxrpiib.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/geshmeouv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gniabfxdj.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gpozdpcpl.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gekfrhwdm.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gpvpbztqj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gciwcvvjh.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ggjgtunxd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gdliuuhzy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gygicadwy.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gbxmgfxyu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gfcbkwfge.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gnkeiqlaf.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gqvpujsjg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/ghecuozgl.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gyjwufndu.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gprgurenb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gtuanayyv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gjjngijqc.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/grarekbdl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gweznhqvm.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gikykobmr.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gnxdpglgz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gkrovtrps.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/giylirkoq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gjcepmvpo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gnbhveysu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gzbepvuru.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gylgawzqv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqwvbskgi.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gxuseasqc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gvgjudgys.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gaswumoie.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gbmyssdzx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gwymcsjod.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/ggznlkfok.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gapyepiwd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gjpuwukzx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/giqgeyclj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gxlhobyty.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gufzybdfx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gwupsjbnv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gkurrdqqf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gwgpivvhm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gwgztwcdu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gtragsuxd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gketfzsov.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gkfpdynap.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gvvbklbzy.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gjiujvjpw.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gyalkymvf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gsbjkgwuf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gprcttaka.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gpoomxzfz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gnchacwau.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/grtcwcmwj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gvzmwhwbh.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gxehfnhrr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gveybqkbl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gpkjqctis.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gobrszcml.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/giaiarwhb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gerzsrwbg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gquktrfjh.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gthcqsnra.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/ginwvkxye.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gxvcdgupl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gwykilufs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gkmhtaqkg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gukptmwec.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gxwsxuxez.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/geuezrkgc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gwmivxphz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gfasayyzp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gczebtjlc.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gqwstmawv.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gjgfqufgk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gdijkoavb.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gcnrdufrr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gakavcavi.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gpqsdtsck.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gzcmxiwbr.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gtyrbwumf.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/ggakssmwq.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gtvsmmtab.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/ghfputhkn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/ggckamuwg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gdtletjzh.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/goaclifnm.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gdeitjwwk.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/ghlortomd.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gitfgicks.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnmfxnasl.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gzjrfryua.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/ggzupqhwb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gbybozfll.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmqbzvahe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gnoqzakqh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gnpppqavg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/goxsqtcxh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gzoyalrkv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gqcdxtdzj.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gfkrrcjzf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhmyhsuy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gwddcaehl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gcxmnrcnh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/glljvnwtp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gbqyeqjtz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gicpftutf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gigfhrtlk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gdfszrivd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghtojqiuy.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gmpndmczs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grurqdsax.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/ghhmhpamc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/galmparsl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpyqoypsi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gxurpxfzu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gdlnhghmd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkbvrhvnx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gqbhdzksf.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfknpeddz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjupncmmg.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gczvkvyld.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/ghaypwocg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gtnxtuzdn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gwmcwliob.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gzzzdprzf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gmuhlfuxj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gdmmqsoqj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gonoyqwnw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gehgjnjgi.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gaxwmfnka.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gjeqoeuwl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gojczjrqq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gnirycwrp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gicvbmiwo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gznditqbs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gifrfskxo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gimdsnqcj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gikecenhw.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/grxterstr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ghncpnoxx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gkirpemgn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gzhabcjvw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/goslkaonm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gjvqvgxdh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gtjwsgjpy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gdspdixgf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gjcktzvpg.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gktepbjed.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gblppzklt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxxrxxxyq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gciunbawe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsmfxtrwe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gnwzxxogn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/ghbqqciai.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghzftqhie.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvnrikuxx.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gidkalczs.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjtxkupsx.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gerljzncw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glerjhvng.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbouoltkx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gvxqxnnsn.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfqrepxni.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwcrputen.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gkpeaquju.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gorbjlacn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gdaudprlj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/ggpxmjroc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/guhljzvtk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gempwbvqh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/ghfhdclsg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/ghvzwxpec.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gktamfxuh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gsogodbld.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gcabexouh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gshgzkzcm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gdlpngsyl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gehjysabm.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gcenqryyg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/guokmriad.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/ghfxvyrdk.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gdvmkqaoh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gfypnwtom.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gqerwqhsp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/graykoifj.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwwwctfjw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gajxrbbjs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gkavluxut.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gzoxgupdy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gndfconnp.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdvvkmhln.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/giqmbapqk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gihyxelux.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gadwenfez.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/grcoleykg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpiegmlqh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/genucgwtp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gmcuandlg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtvpntmxe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gygfsrbuj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmfbyvwhm.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/giseswfto.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmzzwkrcw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gvglotsgp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gddzzgfri.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gijgvoirw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gpmexfggu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gfwrxyeor.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gllyhgtgm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gsnmemtxw.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gxsflmubm.sHtML


<!-- 参考信息 -->