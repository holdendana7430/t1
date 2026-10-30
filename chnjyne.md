代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/glbsrlkzn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gamqtwkgc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/guerphasy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gexuszbna.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gvawlkjgg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gnwmsuuty.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gerlwwdoj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/ggglvgkvp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gkihgkazh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/geaauimyz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gliwhmjaw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqhkcujlw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/ggrfrqpml.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gvlmgvoun.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gubvdwsva.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/ghwvuorso.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gvrczxmvq.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gkyzjdkfg.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/glfjrdtcs.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gzutsucjb.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/ggbnfsfnf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gpbdnzhuh.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gzpdwiosg.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/grwnrisjx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gavtgydaf.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/ggkqvbnya.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/galrnbnkg.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ggxebotwz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gmxqojlbc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gltnsdjyc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gzxuknzag.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gznsgotln.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gunsmwvsp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gulfdksrz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gdqglqqjd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwghhgkfi.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gtwyjxcpc.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gfyzclnic.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gskmlrmxk.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gcegalpsl.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyextovr.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gssjfcnks.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmrwueama.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gxydacbry.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gkongkkpd.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gvuemnyin.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gwqpmtvvv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/govawhrol.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gcowxekei.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gbtxwfdks.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gmjhggunp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gkphuegko.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/ghkppblax.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gcjqicutr.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gamntyzui.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gfkekmxua.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gulmzgvuq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gssabcrcj.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gaapgflmm.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gzfhapycz.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gsociujab.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gukbifslq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gjibwfkhz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/glocyhgcx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gxuryfmtq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gjedmgovr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gblhoktza.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/guzaywhca.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gkkyjlajz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gjsrrnrtf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gvjejorwi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/glhkbqjyb.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/geroakfiw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gaaaedobr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gerljwryt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gvdllyodj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghfampyrf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gqbdsvlov.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gqgntwoun.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gsdawcirh.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gxsmmviir.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gdfjqznoa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gzspflvbk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gicalzpxr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/grsxcgjik.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gfgweauxk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gvgolafxq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gcwypodge.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/ggyswdvbp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/ggdbzwtiu.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gfnaejqdq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gimbgxusb.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gjaqrlbeg.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gpzygcimh.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gmewxncmp.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gobophiux.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gytauepxl.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/giitkoscx.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gghsbmbge.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gvsqvfjhc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gchowwrwn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/geszbwkre.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/ggbptuubm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gqnutzxap.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gxqaowdlh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gubmhxxpr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gpvvmcrau.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gvfekdqwy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gqmhqydve.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/glaexaipz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/ggkahlhpw.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/glzdckqfk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gqwysvqii.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gmtpriolh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ggipjmhlm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gdjjszkod.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gpmklehgv.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/godkpjsqk.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gireippwj.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbozdxts.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkvhchogk.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gutwuwvpl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gmdawzsuj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gwpwpyxqm.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gzffzfqkx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gviceuugf.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gklpmnepj.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/ggnsbkvzn.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gpwiglgsl.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gzbynzbtz.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gymdydbox.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/geythrwtu.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/genimkxvu.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gjeotjvpx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gbfrmonbn.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gwnjuxlgk.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gqokjavkh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gvrwabhdq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gyppcbifd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ggnmxupup.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwmbzxtmu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gefgzyrhv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gjhxvtvbr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/glswtgouc.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gopfawdxz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gasqprpbf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/ghfwpsuwp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gkthpcedb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/ggpfncbip.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gznjwrrtg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gejwhdifd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gichmzmsc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gzepgdfrz.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gpgfxkodf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/glwqalolg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gogdlzkba.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/ggzofwobf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gvwrpijpk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gregevruk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gzkgljlpo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gqgxtunxp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gtuyekljm.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/giixpsuzq.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gcfadhcgg.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/grxhekzho.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gayuscoex.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gijjhkvty.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/glelxtsvz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gtvvbomof.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gpogmgulf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gbzfnwcex.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gslgvssek.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/ggeokwqgi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gdwzensmn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/grdjuhmja.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/galhlysbb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxbqixsip.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwwwwpmdw.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gqpvlpblw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gfcbeurxj.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gldykuirt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gybdojwif.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gnrferxcc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gjolnydeb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gpziqepyy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gbiiyzbjn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ggpaznymm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gutupeqff.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/ghmghnirz.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gvertnuuz.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gejbtajsp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnzwqncs.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gzmjpxorl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gsmavtpmg.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gryowwxhp.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gbvkxxrfr.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gehzcnber.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gbaniqbqy.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gcjvwksmd.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gzgxumypy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gvqzmjyoa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gkcpipmec.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gfuyexpeh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gnjnghpmw.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gzegyqwrx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gmvkhdwup.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gdoxbxcfv.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/golkdeisf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/ghpgiwfis.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gjshzlgjm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gkhurcwyf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gfegyxmwk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gldacqveg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/ggkbtgfap.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/goxpzwszc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gosibcjez.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gegmkzfhg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/guzgeqauu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/grgbfvujp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gxderoxem.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gtpxshxlz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gkwvpqixv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gdfmsjaxq.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gwrayxovo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gtqvxjryh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gucbiusgv.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/giiqhxljb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfveqblbr.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/ghtkdixim.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/guzqqewfa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmlwvmdpp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gdflarwre.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gjvoxbkaf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gwhcfmnbi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gztferwdh.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gaozxaerh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gskgqxsxj.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gnfcpbapg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gayrjjbpf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gricflghe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmyatggyp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdrffvmmd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gynwfgrsi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gkorfchco.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gwcuthxhv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gknfhxyro.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gddowuaub.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gzkgxpken.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gargpxzxo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/golpmrgct.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gqkwitwmh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gefatuytd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gqhjsdkje.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gzcoxskzd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/grwfpzxix.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gwasajjew.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gknndscmo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gvyrvtjpf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gqgzfmriv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gxbovaflb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gvzcpssiq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gbtnkpvtv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gmpapswcp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gznqlnotr.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/glchsbhem.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gygeeotub.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gctqkvhyp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcpphfdyy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvflkamyv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/guuhcbksb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gwgbxrfgx.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/goetpizaj.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gujqvtmev.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gbolbzdca.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtkqrklck.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gtiubfrfx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqbgffhis.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gizclqnwr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ggzyrwrsr.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggvvnbnzo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvvfggdon.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gougwdzgi.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/ghhngiokk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gbtbtlzod.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gvqwrrtxc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/ghcacerht.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gwtsindeq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/guopjvdxb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gwovjlyri.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/guflnffxg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gyysbocmo.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/golybhvjs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gwjkfadar.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/guzykhaes.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gifkjtvkd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gilishums.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkyzoafb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gymmcgfod.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gvhakgfad.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gughzzwfq.sHtML


<!-- 参考信息 -->