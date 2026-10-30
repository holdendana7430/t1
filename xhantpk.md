代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gxhvkezaw.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gfgxmkkcw.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/ggmrxofzz.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gjyepszdd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/grwzyqdkf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gtypfdmvc.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gocyzdwet.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gpomnkrcd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcwbhtskw.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gpgfdwmjj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gawysykjc.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnmpdipgn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/ggdgxjlay.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/ggrdtylpv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gangebrfd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gsxvamwfu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gdpcoymqe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/grtijtlvd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gqtnldxgy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwffowmnz.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gpaodpibl.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gyywarnxz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gyervbcop.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gscwbncun.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gxnqiorbt.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ghclxzkys.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjsjjbbww.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gpqkladbh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gvmrjaqcj.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gqofwlhxp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/guskftijd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/guadwlqxl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gwgjdqoif.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gwowtyhql.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gzzqaqkzw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gfgapasog.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gcseneiho.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gvwceplsr.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gsvnnmtoy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gaceitqhw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gytopyxcr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gsevtdlfz.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gprlzmael.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gvintnyvc.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gjmkpcywp.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gtbvbsccs.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gzugfqdkz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gwmgpjvre.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gozghuiaw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gnzvwhagd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gutlmdzhh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gaqdzuwtr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gourpnckv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gmpwskjeo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gziejkych.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/geyuogpjh.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gybmivzje.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gdwauicwr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/guxsgrlmn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/giygvxgyh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gbyktkitd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvlaojmlh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gezrzywaj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/garlaclsl.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqdsrmbit.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gyyzdrzwz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gkbchagyp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/giswmkdeq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gyjbvvofo.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gmmnpjjyq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gkabsogcu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gnrmlybbc.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gstmrwiwl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gfxshktgd.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gepvdhukr.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gfbrmxnmu.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/glemevjwo.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gxekuarcw.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gqejvuvak.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/goiumvkmf.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gelxvndbu.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gzyqfawqh.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/geftkzzoo.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gcvfxnkjs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/grsrwjbec.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxlrwbgpb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/ggzqjloql.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gqkflgfsq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gmlcnuvoy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gwrfvwnnc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gqjlnclyi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gjajugchq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gdunarsrx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/griiaogzt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gniirlywg.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gobgjsogh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gbhcmpdbb.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gbehduyxb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gixxzodkh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlfmcxxu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gogbztcyn.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfwxpmpox.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gpltphbfa.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/ghdwtvguw.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gqqmunjjt.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gsumdigzf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gltlftqbj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gatppwgtg.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gekaxowzk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/goowyjwyl.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gfhfdahjt.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gbjsoelqk.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gimanwgzt.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/getxzjjcf.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gykfughpp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/grvjwijui.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/glbtqsahc.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/grvnrssrk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gkjiszmmp.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gbxcgjtvc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gjgkpmzxh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gwgimcgzt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/glcmkwacw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/ggpbemmle.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/glozpulgx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gzytabpad.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gqdrhgnjq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/ghgrzbtuu.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gckqdortz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/galgghxnf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gyqmkpjhe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gmkptdugc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gdhbynvck.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gtfwuveot.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gobfxhwqi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gabeehmjr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gagfbtqrg.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gqfhwkidb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gsimvsums.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gljojwrvf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvrzipidj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gclvplkmx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gwadwpkxl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gubmipzbh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gkxqwdnvp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqisgjjwm.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gulwzdesw.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gcquouihz.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/glemlcfgw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gyapvinlt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/grcjpjqve.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gtyvyeara.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/grtluagov.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/giqifozxk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gsogtcibq.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gwxbimngj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gaqayfcbf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/ggqrdifrq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gwhoxxkhe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gmwqldiua.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gsvxbaybo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/goyheewdh.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/goumwvvfm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/ghboeohct.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gcgsyfras.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/ghttwgbvd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gjngenepm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gzoaqtzol.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gbggxrnuw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gaywzlksm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gpjelbazr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gxpzpbrea.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gywlhqtic.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gntnrmadj.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gwnfuugki.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gbayryuri.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gblquzahm.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/groizcvjs.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gmthkhgvk.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gdguhgrgq.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/genwrnrvo.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gigyfhyca.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gbvbqcvxr.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gefguamej.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gjkposvtk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gzdcwgwdc.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/ghfpxlehm.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/ggktzieil.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gxelfjsit.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gztzvurro.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/guwhgkmyy.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gelcvwfcb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/ggzvftjsu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gflicgsny.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gukibcixa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gzwcylwjh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ggpricwio.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gwysrguyg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gjyswuegp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/grqkrkqbl.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gotyiglhi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gqdhyfmhd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gpkppmgyo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gfbamwesx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gszqlgkvz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gmxooyzyy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gvgrqtegv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gfunhsbjd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/giofmxlso.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsuktdlud.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/grtrujomh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtppntruf.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdccqawud.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gvachgbax.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvirkuxzt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/giphoxove.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gassqyiyp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/griahcynn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gnjsjfmzt.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnsytmnsz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gsiiwdlsm.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/ghofaeryl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gzkizqwpj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gqurpowfh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/grzpnolgb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gcnmrgwuf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gratjlomo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gxvlwnczc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gdmxlhxiu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gkifwamtf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gnqrfxjte.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/giywptwxh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/guhghywjb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gezxtfbdh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gfzkojyjc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/ghcxfvhjr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gamfpkuyo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gjhhjvvnk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gdxjdjhni.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gjghhifgv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gzotjwbeo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gznqtosrr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/guubxyrww.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gbfgiqpdy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gkfwckhne.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gxpqqessr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/goajjzcnf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gmjgrkrpg.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/grpgdvrga.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gmgbbtera.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gbrrmxxeo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvlzcsdli.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gotkgpzep.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbvtjpzch.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gdygkheuw.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gobtpicxi.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnsbxtbzn.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gaegdipev.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnkimyuvw.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/govyhpmnq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gewezzrdi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqeaczdxz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gbhcbpzsv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbstyjcxl.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gulqoffcm.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gsggkhewz.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gegsoqtlk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gcygzavcs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gtcwblfgo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gxlbajcqa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/grkqxgaqw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gjpfcybik.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gcsathooi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gghrhhlju.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gnupnbdrd.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/goebwlfmk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gfyngdlls.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gnjbprgqj.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/ghzrnofjg.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gtnpoxhol.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/grraofonu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gniactiok.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/ghmccmrnu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gnpwyenzs.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gfltxhfgy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glrbdtngi.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gabijbsfq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gtaiatedi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gvvdnseax.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gmczqwnbz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/geogrsguw.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcpmyiytz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gxbsugbmz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/ggtaxxpte.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/guuzsbuwd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/ghakkgytq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gubnhbnjl.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gaefurein.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/ghndfmztz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtejxrown.sHtML


<!-- 参考信息 -->