代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lvtabguf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hoorcdjx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hcztbwpb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pcnaxkkn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ttigxnja.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2eogjesnb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mrehllot.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dsinwchb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zgzgqxiq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mfkinuxl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uisdooit.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jiomuysi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zgbpblce.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ssprpewu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kjgnkcab.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jxbtpkjg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dskxdapu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bytybyyn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2zemftwmt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sruxaxae.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2swvavbra.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ztlfsoqk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ghiqcblh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mszgbjpl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2klmerxnv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wpsrdneu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pfrcsrfn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rcdeddgv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fpmstycr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cusoagpr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vednzmcw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdffzhaw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2arjbcpym.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vcjcnouz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2sahsilbp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gkssydad.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wenepjqy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kalgrtyz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qziydczs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ajemnlis.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qlcyoqau.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dbrbvkkg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jssqpgsa.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dzqodjon.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gglyfxrv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2npwjsykc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uqhnoyvc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sbyrtncj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2oheutrkd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dutxqccp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2iqxsjcfj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dxidhukw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wktzbtxx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jtwrrxrt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vlzdhjqb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jpylldlj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yyvzkhky.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zeutumcs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ncgbdopd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pigccjww.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2rymbaksa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2agiyjzga.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qbzgxzes.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ggjkshiq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yjthichm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ecehsdgp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ojlvojst.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qlkcqymj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vyihbnvk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zoopfkjd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zcbjhryn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bxmhfwtx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ltrhytca.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qpplzumq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fuxbanhr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2mnrpuync.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zbchripm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cnmdtryl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2jmkandqm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oybbkbxu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ombilhja.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwoywkxk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnjvqrtm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zzcncqxs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ejotewpo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wkfdewvd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dyjqxtfz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gwzubntz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ownvjtlb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mdzvzqqn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2anerqqfz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2pskpvzwz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pbqgouci.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pkfthkzn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hhpfsnqe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mpnrtshf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nindirlc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2oaoujavl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2sfacjlpp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wcwndevz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qiqjzcbc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2yfzienga.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ulhfqgjv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2sjuodthg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2rytdrumw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2gtefwzrj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ylicvjbi.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2icpcjonx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kogvkgkc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jnvbijjs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2iyifqqkq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2txwumijo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2opeovpzs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uivcdlng.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hxoazxgx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2phbruomh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wyskmwpz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gwanjnen.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnpdpohe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpyjrsvo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2alnsozxj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qfkkpqrt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2peuuwdui.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ertqlsys.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2pbzrdczp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2sevnxjir.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ddlqjzos.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kpxsssbs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oebhcerx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wmstiwye.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2udbmhprr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ovoufehc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rdxuscqm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ydvxkijg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xdncjoez.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mzsvlebk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jxuzdzcc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zjxsuosi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ururkvwi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zanjfauj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ssaeqstr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qtsxsfyh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vzhpnjqy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kfolufch.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2feozlhww.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2geozlcdc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ayuukfpk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofdgklpx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ceouxwaf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2heccnxqs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2amdlsmus.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2uladafcz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ckxttdjs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lboacgdh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iisjrira.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bjqnevps.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2naceqmcb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2nvapfdkk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bbzxtbkt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ywcvghct.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tbwmbkoy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lqjdbiwh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rrpeuncs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kvtfcjuh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wfxclwvf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ceivfjtz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cemxqlrb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fmcrmzgw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ygizznnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aachbxiy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2pvajtizp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuenrrhi.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dzpohbaz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zbarkfsi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2idnrgxil.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mdgdycfh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2paofndsv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gjatebwy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jnoqsasz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cscmfmrx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xnopwynt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ishmypgw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fxwlarzd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2sbvyapwo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vgsyyxtt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hslqrjyr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sizbtqom.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2awyhoxig.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hhndfavy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2epdmummf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ghoqgkrr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2dsbgnabt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2apmxmtth.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uqccicaj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2koallmup.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2opimbrea.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fcxolumx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2orchkrwm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bouwbmdi.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmbdtqhr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mfmdnded.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2bvcwfpoj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fotkdmir.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zbozogzc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2javlplln.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uillagjs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2msylqwbk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2utyudrta.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nwfmthnl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rgeyaruz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hnvcusdz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uuiemvwd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2horeswbu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bgbsnblr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2cdloakdv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uejuwhxy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ehzjrzqz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mkvfpuxc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2anigsaxm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rykflijb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncyweydu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qsuudniw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cbqqzimz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eokdocvq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yirtszyy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szcldjiw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2sddftyto.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2omulxdav.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qqqowrjm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2impedsuv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gnbhqmzu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vhzzxxoc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2viylxkin.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cztcxopl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bhygafnj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2hhogsvjg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dvbhvzqs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gkmaihkm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cvdbbasr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qupnwcwt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gwnepirs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ltovcqte.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2hyaonniv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2aavoeogp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jkrskqwy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwyemslg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ersmhbtg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oovptxvl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rdodfmfv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ercxrhxw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rksggyss.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lalelsxe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qwtvgiyw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2uwziaiqz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjquizut.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ruwyavol.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfjwpqaz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxawagsf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xnhvuzpd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzavdqik.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbpeixqr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rqezhmkt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mvtxrcju.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldnmehsl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2mafkxlso.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjiqmuok.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vsgyadvh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cnwpapmu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2huiptbre.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iknzubhc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vuwrdvlx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2paccjxrg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rttwtkwy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ipepfaec.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vnbpvnqx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zlahnsyd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2tbjqnfxr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2mziahkee.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2oentlwdh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2guenchhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqzmlnza.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hxyltrpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unigngcl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2fnsnfnxh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rrhljbyh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ytnnuagd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lroegzxu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxdkwnkj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzkpzznn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lnvmzwoi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2agrkssfm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxnwahue.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2abkmfoqu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2pxtzqlvo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwcdhtua.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sdiummte.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvrpvviu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvcdmobk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2rqheuirw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2umeokkzj.html


<!-- 参考信息 -->