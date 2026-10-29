代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gfhamcoen.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gkhubfrdn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gqstfezvs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjvhktce.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/glpjjvdgb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grkhwsjjs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gaqkabfra.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gxqvrmbbe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/grdnyfqfn.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gsllmgnbd.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gcfcadnrz.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gtobokxqz.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gukjludbg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gpbkwfdwi.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gvbegvpbn.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gxlyswrva.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbzjcnmjh.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gvyntpbke.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwuczjgjh.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjlgtrjfc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gqltxcozb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gqrrgnwdc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gstlgpqbf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gnukqdbzx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gqdlzzoea.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gtchlbdky.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gptiwbbby.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gckegprdf.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gtjzyimtm.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gbbkqtltb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gzcrgcktu.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gcyjbfbjz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gswskxvpj.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gvlfkpinr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gduonqmez.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/grmauiuhf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gyhtmbwbd.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gbhplspok.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gdpbzrrvl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gdxgssewo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gwpnfruvw.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gbatcflih.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/groiktnrn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gnutgrqfx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gbdodmygb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gnubzpqeu.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gqwuemxoh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/grouaiylu.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gdzxcwgsv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gqmiuzqbc.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ggqdeibis.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/grkuyhpiu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gcflhjzvw.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gjhzkqbdx.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gztqcpria.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gkvtzbevb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gnmapfdzk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/ggctcbyoi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/giqjptdhs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gotdilnan.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gitdlcvxs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gjuxrpmxy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/grqeewafl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gdorvxkib.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/ggbspgjfj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gwsjohosc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gtndufgzs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbfiawcbx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gmjydgegb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gvwpxgfer.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gavwsazhn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gwtnzkoox.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gnmeclkmf.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/glbndftey.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gcxejtqvy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/glhoyfzls.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gnofrsljq.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gqvvmbjjp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gvrkacmoc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gutldekmu.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gcvzhcnom.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gvkyryzpp.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gstyedacd.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gnjdwnvqk.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gypxshghj.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gugmpskrm.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/ghsbmmwdd.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gjzaatacv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/goffttqat.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/guszjojbw.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gwzgpmabi.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gkolkzlki.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gtobplkxr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gjdfjfeec.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gmptjhbet.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/geqvyaboa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gzfhbteqp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gagglvzpz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/ghaelmdls.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gzdtunaiv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gkikrgyob.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/glmpbsgbh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gslygdejb.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gaklwgcra.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gdnkxyouf.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/ghctyniph.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gsyzopcoq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gboluvwcd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gasrdtyqb.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gkdwnonyd.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gtkxmxrrg.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gxvlxchzr.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/guxuqtbzg.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gqstfqwkx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gnmuuixhm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gvypoeawo.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gtfgpakul.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gzkyilloz.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/ggyxlxgwo.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gxwnulpwi.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gurtfayck.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnouqfray.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gejaayylf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/ggqofiuze.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gpjhrlzkx.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/goxzmbmcy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gbnxakgdw.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/glhbjdsrt.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gkaenjsob.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gwkaxhaqt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyzndbqgt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gdasaleyf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gvolflohr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gdpltviga.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gpmvtiulj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gljnyafro.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gjbdgekix.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gqvrredzb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gzwpfbeya.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gvahvqbwc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gykhbisms.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gffwmaizd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gcrirwswl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gjnxccrms.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/grqlterfp.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gyoexpbgs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gmpycmveb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gwukllnjx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gzuqifuch.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gycuabdev.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gptozllfj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gjhlrieib.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gtjpzgjfs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gipkrusnp.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/ghhudqlqi.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gibfxavdg.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gjzfruhcd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gscolqkbh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gnnqnkzor.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/ghjwfszqf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gyzziwsyn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gkmstftsr.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gqjgpejcc.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gbhccaewa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gzjiwfzkh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gpabwlzhd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/giiuokbms.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gydhltpok.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gogggbuym.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gjuemzfai.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gbdatgvru.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gxssdvmbc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gdilipzgk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gmxrxqynf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gfubxfmvi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/grjvlbuug.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gwbfrsjpa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gqbtxvlfa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gxobkrtha.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gllfjoalx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/geovlyhar.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gvzebuonp.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/ghcxwkydo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gopitatnn.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gdrzsoaxg.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gwdeeedav.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gquffztdl.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gfmpodtly.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gjdzjtwnv.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gycxlfplv.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gvaortltk.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gcfnrnogl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gskpklahm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gtfknciul.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/ghzwsrdbp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gwzgwhzge.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gquufhcyn.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gigityqsc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gmqcdrefo.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gwbkwoxbr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gwdpfjkrc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/geoktfxva.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/glqblrykt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gybhbmcoz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gzaqkwlpw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gyjxpscmv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gykstngzh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcicplsgt.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/ggnsvgatr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gozslecsp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/grldfmjyr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/ggrjspgal.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gasnxopub.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gcsdivbma.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gvbkvdynj.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gzzbtkjml.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gvsyoshzj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkseeczsl.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gprwwogvz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpzeclovb.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/grrnaeoks.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gpfvxfeto.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gczgitjlv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gdcavageo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gdjedptud.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gtsbiqcto.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gbxdcsmwc.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/grpbqcakf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghhcbgiee.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gaycmrlsj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gorxkpxha.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gkhhgepha.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/glqyidgfo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/giezdcbfj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gdtrwjjts.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gkrhbxyad.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gxculnkyi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gcteyxgyh.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gdavpvrhz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gqwoxmerb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/guzucefwa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/glwcsgkws.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gqtyosjju.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gdfresfwq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gwgkyzqie.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gogiqzjhm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gzlczlldt.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gzvfdhjjo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gsjpxfxca.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gxwyxkulg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gqgdlppan.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/ghtrnkfke.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gssddedxp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gqudtewng.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gwttwodaw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/glouvupxs.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gvrtywrif.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gzumyprwx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxnletcfq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkwwhroxi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbhvdeckx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gzsxokhea.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gparyzgoe.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvdpoccup.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbvtzhqcj.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gmsqiifjv.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjfjgavrn.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ggsjuahfd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmzvvuqxo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdqkzcqmf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gqpqgpite.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxglegpjz.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmqlikhwk.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gnwaoryvr.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gupzdohus.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gmnshtaib.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gmzylgayo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/ggnodeooe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gjrnoxpyh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/ggeuyltsu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gcxujneqc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gjcviugui.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gywqkfrxl.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gqljfwvnv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/ggeblyndh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/ggcfksujm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/guxpjuylp.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gmmiassvj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gifrowqoa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gjsdmceun.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gultryiul.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gfenokehp.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gfdgkrbjh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwvlntxdo.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gczmmzasb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gyytmoubv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gblxizgsh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/ghlduuimh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gizhatsqp.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gausuuvhl.sHtML


<!-- 参考信息 -->