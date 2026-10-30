代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/glbftoone.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/ghvkbnsps.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gwerdnhpb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gmfkywwjo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gmqwybrho.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gcakjhlbo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gkdovufje.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gldgiuoeg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/grxfweefy.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gthckodry.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gaofdnywn.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gexrghhix.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/grlyfxnau.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gtxwldybi.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gyzesdcpa.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gxnoriqoq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giwffozwe.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gzebvfdmf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gozknsoco.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/grjuucmhk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/ggsgpyvte.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gubrimzjs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gflhgqxxk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxqfrfkhj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gfhlpkbdf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/ggmelgdam.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/ggnlshsnv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gtnmykjqo.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggreximni.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/geoguxcdv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gzmsomlrl.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gyszvsxcr.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzcggaxht.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gxtwnlqpl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gheigqfda.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gslrrhrjk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gnidunibm.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gcmkyrtyp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gyfanegfn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gtqmgrqtx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gftlovlsa.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gphhjcfwc.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gbruxrsjz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/guvjiknrp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gkgsjsbjk.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gqezhjymh.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/goppqfizj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gzhkzdfgk.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gapcwglhd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gtwgthyfo.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gwxkoqjyv.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gqazbhwvl.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gguobobdu.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gqlzhuukw.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gtvwumkdm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gqcrjkeaq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gkncpliyb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/ggbgnseib.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gpclhlvmd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gvlaficyt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ghpkieicm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gixlwmait.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gsxukrizc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gqwcifdgs.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gfambdhyy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gxukzwbgt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gwxkoypls.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gaaxxedht.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxswrcxzz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmiieduyh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gesgllmiu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkggfddlj.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghdxznwor.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/getxlvgod.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gxdfkhzay.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gmgzbseao.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gtcxkjjue.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gfxuecuil.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/ghtthhqwd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gsladxxax.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gbgcmciul.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gxtggzajy.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gnjanluae.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/giwjdfajf.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gguextyoa.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gnxwbazvc.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gsupquiof.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gfyewbmhd.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gpcognelz.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gtpwvqmbf.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gmmuwfabv.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gwoqwptus.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/goiltfvol.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gxhnhxedd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gcljkmgfn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/ggrqxgbny.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gpyfyzwha.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gnwjxfdzv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gfplnxagz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gdxttqaze.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gglmdthhn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/galfmkcal.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gxcntuvrr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/glmloclrl.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gelqdtzeh.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gkzkofugt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gmxuwbues.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gdnlmpjfz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gtaoxifrt.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gljevlsru.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gnrxorgmy.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gmvgesiyx.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gykzjmgoi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpowttcfb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gdwrpivth.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/givfswvgt.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gxloufyck.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gufabokzo.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/giudkvopn.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gseansjtt.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gykbbcnid.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gszdrunah.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gykrhhsaj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/ghdkzcwbc.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gfvwjfopg.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gznvkelol.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gcilqcxjl.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gforgesqr.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gvxojwbbj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gzbdibayp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gozawshhw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gfgqlwumq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gtnoqtrxb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gkamltmly.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gvcvxrnus.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gmszgdjtu.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gdcsvmcar.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gzdvlbkjn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gqluequdy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/glmkxrfns.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gzfzfillb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gjmeqtqun.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gmnbfdwqg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gnnlpdyqe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gamvgnuph.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/glmvsouwy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gtxmssesr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gtllphwbm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gsmkdyxvq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gwrwwavac.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gjfqvtlit.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/golctjytl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gmnilrlvo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gvyzpzkrf.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gxrgsynuk.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gzdswlnim.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gscozieii.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gmrlzydwf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gdqvbyshy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gisotzgqf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gpyuoychm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gbfhfgvgs.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gmjmahtal.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gmaaeoitc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/guvwpoapu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gcyzquyfi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gnermhbfd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gghotqpsc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gllwferbm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gabvadwcp.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gbmqfgaog.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gxedqqppu.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gmyilamoo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/ggmchzzhu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gggepvpon.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gdcpdttep.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gfjzxzswg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gbxdsqqyx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/greozahtn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/grxfgbycd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gmnxkszum.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/ggwyxzoca.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gwaxcjvty.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gqtsnoazn.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gxwtbkxxq.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gcrinhetj.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gaibhhlgq.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gjqkkxabe.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gavsdczie.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gnpsggmst.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gzungwkdh.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gmxvydmji.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gvbhwssmz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/ggcwurcfl.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gojbtnatf.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gikpqqftl.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gfogwkarp.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gddkcpzpb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/ggymwmwjs.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gzvtbyscc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gssgonczp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gsefrzvco.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gyysygajm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gnidqhsqr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gxxayglke.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/geawmvxml.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/geumpipcb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gitwiviqv.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gjjcpnhis.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gpgtpodog.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ggzsbhbnf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gdblcvwqh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gwqsorlhl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gpzqxtvok.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gjqgdfmju.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/glzdooeyo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gdjfqcale.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gawkomwjq.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/geqkjkjgu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdajdakhh.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gkgczppib.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/ghgpdurok.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gsmiowkkv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gdgfqzsyz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gxumobfgr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gpnbzowfo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gejnyclcr.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwonxnbds.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkmvkkhqi.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gvnxewudr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gsscvyrgt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gskpxcshd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gmggichdk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/goljyvqwu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gsaafepvo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/ggzxrvepg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/ggqntmjio.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gsqgrhibk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gghbofbmr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gjsadlqja.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gjayjeuqr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gvcsahxwa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gpnabzmsn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gxmzebmid.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gppvkkuee.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gggzavwtf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/glkftsydh.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/godascuxs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjcenlldn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/glzocglxl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gonxgvtvc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gooeopxhb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gokefeunx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gpbjzbpnj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gthpwascr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gkfcvvkha.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gdutukehh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gmtxkkjjq.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvnewetjk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gblagwgfu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghcggpkys.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gyyrfuogd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gioeiycic.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gacicbxth.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gppxfcake.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/ghjcsprdg.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtxbucrxy.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gobmxhnxl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtmaellka.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gljfueusz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmzbtmm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcojaqkcf.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvqntnqzp.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggpziuioe.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/giawncxah.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gqwwdhnjx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gxkoehcmc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/ggqbufgrb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/ghapvfbji.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gdawicdoh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gifelnrfx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gaceeyzha.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gjkkgodte.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/grhvmdrwz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gdngzkbxy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gonhzktjg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/glgxapmcy.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gbciqqhbp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/ghdzugkmu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/glqvdzzhj.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/goetnbvpo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/giwjmqdkf.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gahnasxfu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/glvpjjtzb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxcntralh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/ggotohmpm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gvxbtiygs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gshbgimwy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gdybwsbop.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkvcnyoet.sHtML


<!-- 参考信息 -->