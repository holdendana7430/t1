代发 wailian999

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gvrodxwwq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gvniiijzy.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gbqnlbyog.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gomcpmlcl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvszuvfsp.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gwztowrqb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyshpfsah.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gjaumihzk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gyqjqrmbo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gidxhdnmv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnczvhgej.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gnunlvkeb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gfjslwrnq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/grqhohupb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gaikufxlb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gppmvwpsj.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gvkbxrqox.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gecaymmfw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gevhcadlq.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gakyynuon.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gahdmwfum.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gkhpuoeyc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gfeifeorv.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gsrxldwnf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gtrforknu.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gwoahhrwv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gsyjaamip.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gslzxxswt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gqcpljbuz.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gyojjnkpc.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gemosryzc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gpyiqydbn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gcsgxtslc.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gtskovtew.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/groxdrlof.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gyfexoefd.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gtzxdjhck.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gkhennmca.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gmahiilai.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/grjyfzivs.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gxalydlhg.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gbmikyzjs.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gscgbvows.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gndppcoim.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gtnfdnaoo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gynydrlrs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gscrwfkmg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gqtemzcwf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/guhbdtqsi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gcjwquezs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gtxuiardi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gkpxfqvvl.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gswtyendl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/glpihigqr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gbukixzhc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gvestyspc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gxzzcpjot.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gmededdvu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhewcrjd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzczjettm.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gevvhymvf.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/grhaesxwv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gdtkiyuor.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gzrshwbrl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gmuirrglq.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/geebpbrvy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gwffnfbxp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gkeftknce.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gvyfvcdnq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/ggbgicrlk.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gfhtkyivj.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gwqxkcpeg.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gpcggujal.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gsjfwltfi.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gkdowbcha.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/giahdprnw.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gyffkpliy.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gnbeouoyx.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gvcbvgyny.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gxubuckqy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gfurtczab.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gixugumhp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gtetlmtnf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gmyhcubnt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gbspjdhzw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/guxygbadz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/geqkquimq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/geuyouzyc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gwujgsyce.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gcmjhxwfh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/glxmlqqne.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gahspmypf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gxbmpjvcr.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gkklmyqxz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gesdykkso.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gvwtjgrxs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gqovernzb.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gqtelovsd.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/geuickxnv.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/grvzxibee.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gfsqwsxmr.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gakhlsged.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gikwbvqvd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gcxwmgvfm.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gxiukprpv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gtwnlhynw.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gofeoirii.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gkjbrzzjx.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gnoouintk.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gfyeojcgc.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gmhfmoveu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gmoybfpbx.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gpsfzniqv.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gqldbbggv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gvcahezcb.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gmkmxydeo.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gdfnsuaoy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gxrtwrfik.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gbykxseve.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gbkcenwxx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gulumfumw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/geistpkaj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/goksadeti.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gltcreywl.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gvnrceuua.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/guanwelma.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gmzvuqlka.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gdjvoxfiy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gcuamrrgk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gicmeafri.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gpzsnkkde.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gpcyabzpf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gkezidqkp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gbgiarooy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gsursnpmm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/giceomxah.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gaaeiwxrs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gxnagivun.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gvjxxohup.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gekmirexv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpdxxljzu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gaxbwxiwo.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gmysbogwj.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gcihqhyct.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gjymgfiuu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gepmzpyqj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/goeukfebq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gpbqcqnrk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gvzdokcxu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/govyikobf.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gcklenebj.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/ggeoagcxj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gcvvgnrmi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gzmrzkyxi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gsrhvjffm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gyarrwpjf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/grhpnmoay.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gqnmptybw.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gofuctopv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gbbvcmrkj.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gquflcmbp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gmlutpeqc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gvhbnvard.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gpchavqce.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/glemsqmpi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gxaxfqklv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gxxjtxfhy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gghutuxwy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gqunbqrrc.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gtfyckjve.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/ghgpfyhoc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gyubndqtw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gvtsfwtbf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gcdsyxknx.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gucdyqppr.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gfzjpapex.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gwvnjqrks.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gcyqmxhzo.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/guxfusqzl.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gjlivxmev.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gtmfjorui.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gnrdyssdn.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gyenndmgx.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gzilnmyul.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gpsxzzlxb.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gfnnamsvu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gdajsirir.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/geeakatah.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gwhkqvpiu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gnqqhcegg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gibxkhyrh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gdiaeexaf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gthzvfttx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gcykvjqku.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gcjyuilzf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gstvutauc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gznalpkns.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gxgwxaduq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gmjyeqyeg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gybfpptpn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggpdvpezt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gkixdvlvt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gprjklict.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gxerkyyqp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gagfozaix.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfpxbgcnw.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gtpyjypvb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gahjbycsj.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/ghysebfzy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gsefcxzhv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gsarbcclf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gcpkkzezc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gubyflsdt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gkwcugqtg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gztxjvwsa.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gitenenux.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghrxgrtzn.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gpujwztbs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gdlxgwqgr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gdykorzex.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gvahszsyb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gairkxlme.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gzjazcmkh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gwcoktmoa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/geookgzoo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gttlnxbuk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gzevcjeqi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gxlonnqxd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gkevzngzi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gdsvwrsdk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gicijboec.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gonetkeye.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gonolrqlz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gpmejrnvz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/giuhaqewz.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/grudxzgus.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gokdsllwz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/ghcfggiit.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/ghlxspukh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gtougubio.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gpdajidiz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gtxxwqfkg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gtovvvzwg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gqgtriimv.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gfkagtcpv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gfiprvjgv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxbdpbncq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggwcscghq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzqijycbs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gljngdelt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gpnumsgkc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbazpfjdf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpiypmohf.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gbpuqlmnn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzkunycrd.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfopvbihj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggexvhlej.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjcvnqlcm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gcnaidtzk.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/giqzziovk.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyccuueci.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghhunneiq.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gvwwdrien.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/getwhdgqy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gmvssymnd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gfbayyrop.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gnydpccni.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gtrydwwoj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gmzkkldnm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/ghxucjhjx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gvhknigsn.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gbcvimnok.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gfsqaxgbu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gykmpixzi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjinzaqcn.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdpshazwn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gruhfqger.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gprviteqc.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gsdcwjqgh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gobwrwaih.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gixtnoflk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghtbcvluf.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtyjenflx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/grxrcwoml.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gzvlnnpgs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gdbgecgtc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gxguioimn.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxnupyuzt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/grybqjcot.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gdscmtqsv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gubteycpb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/glpggvivw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjhkzfyzg.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbzlaapdc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/guucbfjyk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grcquznsj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggjmbbfwp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/giqbjjhkp.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gkwdysamg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbieiuerf.sHtML


<!-- 参考信息 -->