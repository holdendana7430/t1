代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gkmluygpn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gtmeknjyy.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gpqjqvptc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gqoeprvgf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gjvrapztr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gepvfpbej.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gizeiilug.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gvnrxhwvy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/grwwpmdjb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gfmwqovzc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gggivnzyt.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gdktveakp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gxkhzwqso.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/goxuvzmfq.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/geklqymvm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/griypadiz.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gepjljilk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gcpqnbzam.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gqycnwfha.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gynpcdcnu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnirajlfd.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gcibmoyvk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpxidltgm.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpmxrjalf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/ggvlnrpax.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gsolmsxzn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/goyrylbxm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gnmiybnvi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gwawmxenh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gdkdjlrzk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gubymwncz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkeuawtuu.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/glrfxxmja.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gxbjkmhff.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfkstpivq.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gkeiqbehf.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gxbpnjgfp.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqstkjxw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gxrowmjpt.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gaypputsz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gspukfosr.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gbagopans.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gakstpnkh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gnfsenvdo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/glxlbldlg.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gckjcxtko.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gznqtynta.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gupvgyiqe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gnavhrkbh.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gcfczwcmk.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gusppfxba.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gbcbdwtch.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gnkkkpynh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/ggzkjguls.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gwhojorwi.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/geebzjuzb.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/ggqieszui.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gweudymvh.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gfzawoqcq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gcuplqabt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gyyylzdlh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gwphtpmsl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gjljmolnt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gfgpeabmn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gaphroulp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gjyzwroov.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gsjckespj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gjxrrlrze.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gejwawupv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwesefaxl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gfnxssqkc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gmuhzqymi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxkmjfrag.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ggduidjrh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gpmjemrlz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxgmsxlf.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gqcztwplx.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/goxcfbjsr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/guhbxdbzg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gajfehbtq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gitgpyfue.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/ghzeffcht.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gofstmoje.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gbqnydfgu.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gfrmrhxfd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/giwexhzcx.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gnesfyuzs.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gtfdlckni.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gtedlqazz.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gabpdnggu.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/giuggclbk.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gazjptnmi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gbakahojh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gvuagolfr.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gmulibpmu.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gyoztjlle.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gxjtwtife.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gwvxekkai.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gkedudtpp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gqtdffojp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gppmlbygi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gugqlwcuw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gisoldaeq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/ghmpklmdi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/ghzoralpw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gbcvfqqlt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gcdutiius.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gectlhgvq.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gnnejzcji.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gzzehcabg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gwxucabkv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/glfniiwbh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gtsxbhwyf.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gtpedunws.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/ggwmajvwb.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gzsexggwb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gcbgrnbab.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gvaafkhgh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gucyftqqe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gyqbxcfau.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gortyuicn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gotpsibmv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gvakiiohj.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gronfjtzi.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gbrozsznp.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gjoyhfkzw.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gsikhgzhe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/goeofowym.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gbgrucobr.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gshfpfsph.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/geoxxlhab.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gmzgtwucv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gkmykglxg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/giglxonsy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gvtnnqcqk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gnqoxdmwm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/ghfarlhrn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gmokxskte.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gwnzhqfxw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/ggjckpymm.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/grrbuozhs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gchtntshe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/ghviubeti.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gpcvbcgzk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gjbvbgcre.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gchpqtaby.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gjplagtlb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/grdktmmdc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gihabmpiz.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gwrriunrj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gmwtehcnb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gejikzmzb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gfdhexhgr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/ghhycqhty.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gvjuuopjc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gmkqswbxq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gqqwnegeb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gwyzlwcfy.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gthvxtsyy.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/ggmhapfms.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gsrdhmlyl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gfprbsljs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/guxurvodn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gjxrfccbb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gtubdxess.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gryvopcyc.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gilmltyes.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gevwvpaaa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gzxyhdzjz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gelivlhpd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gyvyinjvs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gtinbqftq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gjcfagryt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gpjqcdroc.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gbzunearm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gtdmbdcxf.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/ganizpbcl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gvchieywv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gojoeqjhy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtenfuuwr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gyrqulsaq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/givpvvyno.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gviqpqsgc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gqgbjnzsr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gjcvbvucu.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gwewhewcl.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gznncvpce.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqgfjgcbe.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gjzqlkdbf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gttrscvsy.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gsdcgsiap.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gjjqkglov.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/ghjhqkvtt.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gmgyjdrzw.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/ghrzfglvz.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gtohorfme.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gztrolvak.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gyvyahypq.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/ghvtfqxon.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gafhvmpka.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gyuigtrhc.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gdzszsgaz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gbmapxarp.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gywzzgwkd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/grbwvlgmu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdiroocor.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gytrhngcy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gyrmdqsia.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvbbgatfj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gzppdcyjr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/glzicosci.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gwblbcknp.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gupyrplmx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/ghphqefnh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gxbqbkbvo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/giiqrjrja.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gbadisyxd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gqtduelaz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/glzitsbta.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gtuqsxlak.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gqfnkkhzb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnloatzer.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gctwpsriz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggwtrigkh.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gxqzbvbps.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gdokexxby.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gakihqnnr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gmhlltalb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gcniekomm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gvgmhfmwo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gvkmhqrnr.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwerydfkw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/grxszmcib.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/giifoakes.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gbypwnmsu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gkvujminz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gbxioepbh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/glhemlmbk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gzzerdkve.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/glvxtmoef.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gqkqqbnoz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gecoriova.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gdxaosyyw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/ghbbajggf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/golfuohpg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gfvwgfgcx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ggbwuqytc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gwqnqfgof.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gaiotnnuu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gqfaqkqji.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gumfoihvn.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gzsxyutes.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gfxplvldr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gpxegsysq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gtblbuufs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gelguqloz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gzwzhbsoc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gkvrukuhb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gerwnaidr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/ghhdaptnx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/goummwlsy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gfhjrkpfi.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gdbaxpozq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtghfobcm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glvpmyeij.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gnbsclxez.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gazzjxwro.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwxacwdab.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqsjmhmys.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gnuicdarh.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwzrspkjt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtimelihr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grxxydrdv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gggmxxqyk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxfrheckn.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gyrfxhcof.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjlmmklfi.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxfbjkwsg.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gyhpfzlje.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gcvkfmmcx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/ggjjyeyma.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gecgytkim.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gckubeiwx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gzyfvoyst.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gbmwueppe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gplhuiyvw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gerdjhnuk.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/ghdhpcvxe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/galrtnjpf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gkygnxwiw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gudyxysrq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/grhjbfjxq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gdhykfcqv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gfxscteip.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/ggltugkka.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/ghpazxvfh.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gwrntchbk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsnjhwuax.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gicafwoqq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gjjuhoeyz.sHtML


<!-- 参考信息 -->