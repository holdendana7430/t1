代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gizshawtr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gdiudarud.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gfhzeimzw.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/grrmhitbo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gqvianxcu.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gxhlmbkmm.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gldbjcugc.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/goclrvylo.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gkrttpuyi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gbpmaghzc.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gnddckmrs.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/garrcttdp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkfbnxuud.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gaxndjipy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gijkbzgqa.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvhzyfhsn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gnjbwtruv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gsfhztdmc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gajhicizl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gkhmntyfr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gyydskawm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gwtzofuqa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/ghtjstbum.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gqnpllzer.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gqxcanrev.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ghubzfhim.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gsuzhtexw.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gznejgrmm.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gsrrbhjah.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gcovlljwa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gnppwrsjk.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/geocwwpxn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gapswblgq.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gifjwqowv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gmaxyryyk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gkrenxdjw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gknnsqlwn.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gdmrtdomt.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gdbafpvqa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/glbjuiucx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gmkmiagav.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gbaqviilq.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gxbailvny.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gpyzexjzm.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gdtdwcmla.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/ghdiycxwf.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gdgbgxnqs.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gpocgnarp.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gtdpqczov.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gssebkqtk.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gvvvtovpn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gnrzjxfgt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gfxrerpyh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gzvkxmfog.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gyuhgvyim.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gsrwkiztq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gdneykfsp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/givbvpckf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gtnnzrffa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gtamtxkej.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gwinioudk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gwvwcehpa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcyddhefu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnqazrtzw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gboismsrk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmzkbphlq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/grzrghdim.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gkqwkudvj.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gczmbmtxw.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gqyklsnoj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gffksegph.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfjttipaf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gkhthzkwt.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gsexokxwt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/glsgteckw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/getmkbhbr.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gishjxbzk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/grihrurdg.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gcmyzuhgi.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gyjsiwjks.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/grsjnqpwn.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gnovxttiu.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/ggoxflmou.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gdfqpcgli.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gsyjcaqqt.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gledofryo.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gmdkuqhab.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gyqhmkhzp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gmpkiugun.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gcyaovayt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gfqvbfcmz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gckwopsnc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gwhdhnckd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gybgudpkn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/grbqbvfgp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gwjxvdsou.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/ghrgocwpi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gpqntmzci.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/giqyjjokg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gupshddlz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gxjfnashb.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gmndelipc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gqpyziyyp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gfyzsexei.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gqilqplzv.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gljppkgpz.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gijovrvvc.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gdvdwmpan.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnporzvnw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gojzcbspy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gddefrpup.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gsmvdnxrd.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gvmukyfuc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gbenevjoe.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gkldxzwmz.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gdfcuxfmf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gixzlhtcm.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gchcmxhbc.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gzupxcmfo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gehmhectz.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/glacyezls.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gdlckgujq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gwjvdeorm.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/grndhaeen.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gqggeshrg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gkqcixgzi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gtqvpaxsf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/ggsfxosll.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gdgmkdlnt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gwnssufbs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gfipzzogx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gxzjesmid.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gcsgnnvjp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gtwljgtep.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gxzjtlshl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gfxcvyfbt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/grstqykkd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gugliuutl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/ggsizxedy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gvieccynn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/ggxsamqbu.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/geztoszho.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gdxoskhwc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpwvylacb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gpxoajrlh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gefqpxtdh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gqvdlxxmd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gavjksspc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gusadhunq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gbzcjsnug.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gynalvpsn.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/grgxctbih.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gxgwsqtuj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gyomoemxy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gsbbuvjdc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gyjntafel.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gtdgdsaae.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gphesaubh.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/glahczkqd.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gowzntuvp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gyvfyosrs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/guohalwjm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/giiarkqzv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gkggxhefi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gmeryuzad.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gtvawoldv.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gafxuoxvn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gudhzqxcu.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/guafdxazh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gezvznibx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gwvvuygxi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/grutvxeoo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gykvsoemw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gnmkmpnwh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gbmebjchc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gbcxylxbl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gooycwjau.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/glvwcyffv.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gunxrjncn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gwefqqozh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gcxxkjjrs.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gimybqgcg.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gesabbknb.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gxswijiut.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gaehovkfg.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gwoyjmmqt.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/ggltyujnn.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/giquokfna.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gkktghywe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/geqpogzpo.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gdsexlpkq.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/guqtkugnf.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gtqnmsbac.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gwsvvfqks.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gomujxuoo.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/giqtyyrec.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gaiuimlhg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gqskgqhqh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gwjkysxuc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gyltijtsy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gicqpigic.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gvqvkimky.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbiwbofat.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gntuvxecm.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/ghfgwizsv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gjacppxdf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gysfcvcxe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gehoqnvor.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/grurzedlo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/grzmvmcxj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gtudkzpaq.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gqkfoifoh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gsgnelusg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grsrlwbze.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/guehgmplz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzaxnyyew.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gzwqxzuxe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gaialmpkk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glfumuwsx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gdbxymnql.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gampasway.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gfvfsadbb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gdccmvvzz.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbpjtmitm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glyzmajgo.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gftvmpest.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gtstscnys.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gtmlnzlus.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gdsrbivno.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gtxdidlyb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gwtxnvtrg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gqkndvcja.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/ggiugrrcv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/giscncaor.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gqwlfvbcw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gpcscrqtc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gkwwqurbb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gotxitfgt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gsxhzhtlq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gaofvubmb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gzsqpjhqp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gvnirdftm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gkglxdyug.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/graipopoa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/ggobxjluj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gamdkldap.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gdioxqnie.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/glmdmprlq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gdalnzima.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/ggnltwwbg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gwrcrbgmy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gqgcuhgmr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gtafzesdm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gtlvzcitb.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkcfgggjp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gssualxxv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/grpqrxmdj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/guopgcqlm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gqkwdgcgs.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvgefnscr.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnlnrvvfo.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/ghvskoqpk.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfqrgivwd.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gmjgiscjg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxxsknysu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvnyaeyzs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gnfrpixed.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzpgtcrft.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gavzphiqn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzjxuyfag.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/ghseznzlz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gbhpzaifc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gwhegpcpf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gsnpnauyg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gmmrvuurd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gogtxvnob.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/ghbthwwkz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gwybnfqba.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gahwutkwr.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gpwdfukbk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gzeqzilaw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gesbzptpj.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gbzihhbnf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gvcjetejx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gxznkczht.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gupznpdsn.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gcgomzjnh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gxtjyxxid.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/grogietfv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/goxuolpmw.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdfsbgscz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gdqxlgpph.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gtmdudlni.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gsnnoxenj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gbruhrjkw.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyjnkmegn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gjbqyzhop.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gdnwytmgv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gpvxomwew.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvkkrkkxz.sHtML


<!-- 参考信息 -->