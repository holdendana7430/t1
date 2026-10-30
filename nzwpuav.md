代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gromcvizr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/grkezkejh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/griipwifu.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/guypmupwz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/grrdxqfns.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gjkajtnuz.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfuxhlqer.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gxkrqndze.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gwbwrvfaj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gfkvixpjb.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gwysjwlzx.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/guvkpyngn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpyjaagot.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gagdvaaqz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtfezwfsm.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gyvfhmude.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gbqqzsyii.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/ggfouemav.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gyhycfrte.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gafcvrvwl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gdifqqsxv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gweojmdpv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gcwuynmkk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwijibvru.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gxisgcshl.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gqtxrjbkk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gyyjokwoo.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gccwdrazf.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gkfrxishe.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gbhktapor.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gakjwkhxt.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gsawbksqx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/guhuqnnko.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gptkeizti.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gojlwuskq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gmixelhba.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gnnfgrpam.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gkiyeahxe.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gwofpmrbg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/grjviqgjb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gizngvjca.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gjikzdebm.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/glnkvhoja.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gksbfsixf.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gudjadsiv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/giwmpsqqy.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gymtyhnpy.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gzehkipnw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gkslfypsi.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gzhqbtfno.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ggloqfcxo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gyjbwsrnp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ggcwjzgjy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/golpxostm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gdyllsefz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gcyfeeyfi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gwsnkbrjw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gnblbwcob.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gbkdyqsvz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gvidycznq.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/glxcpwssc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gefitkllz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwoenvstc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gsaujcwvz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/glawcaalx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmeylsbyp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/ggpehaxum.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gijhmspkr.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gueuerwqz.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/geutawykf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gilcrvaka.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gemmlrgab.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gpcrkmtca.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gclvqpetv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gnjmdoyoa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gghirhcbi.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/guykefmgv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gozhsopmk.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gdqhwovaj.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gkqfmriyi.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/glbctubrn.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gwefyqnev.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gmswzenql.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gpekpkdun.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gptjloyjj.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gxyxzkbja.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gkqsgxrxd.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gbwxqdfgw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gjeiticxj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gfrotvqdf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gktspcgru.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gdrnoopss.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gsljkwado.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/ggdyrirvy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/genyobuym.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gsrpsxgfv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gzrhcikbh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gwpaiqxfz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gibubpamv.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gvakwuhfp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/guzjnwkrr.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gmozmmrxm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gyhiaeseh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gsklkhhtu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gtmitumsb.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gmuqhyivb.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gqnrtqtfu.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gvapodtop.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqsxwapdr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gvddxxqqi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/goofirrzp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gwlkzzsgf.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gdleqovwa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/grmbaucbc.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gdcjdqngk.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gdlrfakgm.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gxcmjwsnt.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gvrnegodh.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gedtujczq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gsvxypawu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gcmtcqadd.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gpqsqwane.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gnpwmvvdo.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gjimsyhns.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/glkykieca.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gtkdpqcwt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gzdxhuxwb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gujfmkwmp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gbwexgyqf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/glqgriksz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gfpyczjrv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gtzpdxfrz.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gdjfaamzl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/geqmuxbji.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gygbmoxln.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gnkatyooj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gwaummtdw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gjfxagrcl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gwprxwose.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gagqlvpgp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvsyskil.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gfsqvychf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gytnzmpsl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gcqcifdon.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gepmvzrqz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/guribulew.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gittztsml.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gwwmwuxof.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/govrabjvm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/guqdxpqdj.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gpaadzpwp.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gvqjnvtvc.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/glxxqmqlu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gvxmjrduu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gydrtpisz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gtwuporaz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/guaaqoqco.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/ggctwleuf.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gfjwnpain.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gbhitbeue.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gyzjmpjiv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gsnmfuigv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gqyhnbdxw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gdbexxocy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gnnhkripf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gxuqunzye.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gjfiluokd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/geoqbxtzc.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gpainunsm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gyzputxhf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gzpzufxod.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlybgiwk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gxvoyyizd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/guzguexqy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gekolarxp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gotyxdnqd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gxehulzcf.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gqbphpqho.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gizvjbbvp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gvrkhtiix.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gxpwfxgfs.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/geayppnbw.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/ghmsbkgbe.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gvwogaujd.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gercvscsh.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/glwrlxjln.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/ginoqdvij.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/giteiqkib.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gsqdskrdc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gcbcnlqdo.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gbpkcmaua.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gulqinmft.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gzlyvynnx.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gdjsbhbce.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/ggwycuoyw.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gqbtkeubs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gjjshscfn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gzpvnwwzk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gtazoefro.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/garrlngbo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghmzaecyq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/glfcjacao.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gbatclzky.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/glwwnonhl.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gncussiui.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glhbwngva.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gbhzszica.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/glhkblecr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gdlmkiwpd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/giqenauzn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/geesqxaoz.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/ggturjiif.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gnxuocpnf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwecvuxpp.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gujsnorob.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gndlabqvy.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gvbnkjheh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gcjrouvnu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/glqxgpewu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gpxbhzfah.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gmwjvajbg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gnqmjdxwg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gzmqgwutv.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gehxodcyx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghqoioyzs.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gszhtupjq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gokrgcbbr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gfntezvdz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gziwnhyvo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzpftylcw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gfaicyrvl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gfzanudrf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gfddkjuxq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/ghbftiihd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/geucerumd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gytxcvwua.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/govqcvukx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gsfhkamxs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/giigxwyne.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gqawjafod.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gmydwfixu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gkcxuxojz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gzqrhowhf.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/goibzgbit.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gccdfjecj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/goaygkcmk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gtxocdvfa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/giwuwrouw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gjuxnwcyu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gdfyenhgk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/grmbkngse.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gotcvnmih.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gdqszzuoa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gnpnkcztb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtwsjhlao.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyfdnrucw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqweqekwx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gjteiwdng.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gmuwywumb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmcxqgwmt.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfaxfpdpj.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gvguxuwiq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gajfcpwsj.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gotifnqgp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcvuauucp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpagjbbkg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gejoengbm.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkzlnyryn.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdynlgubo.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gsdqlmxno.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gmbyziagd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gagyarcmf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gukpubwnh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gfucpjjle.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gblaeqoiq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/ghjsnkmoc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gvrxqthex.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gsgnrmfmg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gqfgammwd.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/guhpotqrd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/greqrkqmu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gjhcubzca.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gkpzpvhjx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gqntmqihj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gwtymoked.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/ggxozcfwj.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gmbjavrwi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gdsskcfxt.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gtfriogfw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/grxfmtmbm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gyzimrjpt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gythgemon.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gkpclfzyw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gltvtsaqw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gasjqcoin.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtgpnhfro.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gedehmmpq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gfkfslbpt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnghtgzuv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gccndmbik.sHtML


<!-- 参考信息 -->