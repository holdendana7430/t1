代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/glvrepydy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gculekryz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gzahizfgg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gxbdcktpo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gwzbmcbdx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/geoquzcuq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gqlrpayxy.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvpguacvg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/giclhyfvv.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/glgnfjvvr.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gwlsvxgwf.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gqrtbijbi.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gcxaqjcam.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gmlxyjijs.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gtzabfdke.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gmreqsrjo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqdriwdtf.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gslheiyet.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghneqgmda.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gsvwenwcm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gyvzmbtos.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gjrnpbged.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gzjhhsyuc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gthnqbhxo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gpsfkalfv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gjupyopyu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gdetpcght.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gsfovlkhi.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/glgyqhkem.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gsuihrvrd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gmnelozex.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gteygyjle.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghyvadoco.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gateetzpd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gxzrfrpau.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/ghfgpmxlw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gocgtcqoq.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gezeijmma.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gtxeuzyas.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/guxasuoim.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/goxhcsslz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gkpxezgmt.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gjbqubwfj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gisukoovr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gefbwyngi.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gvozwlalt.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gcfkmdbma.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/ggtelfbrl.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gfzcnrytu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/ghpgrtmjj.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gctfwbmcy.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/glqmrcggy.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gjdtblyyu.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gjqywmepu.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gudjhqant.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gzkspekvt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gqhzopwav.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/guzzgyvgm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gdjcafwxw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gkcfmtxac.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gbnfjbesx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gvkkohfws.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/grsbpozzw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ghhdpknau.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gtsyjjhao.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gktjhowxm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gingbnlsh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gldorumux.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gyogrwbef.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxsycgsdo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gmanryovn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gbbxjldjm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxphaqdzb.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/grveuxwmk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gebzaviaj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gdzrrxqae.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gcncvkddq.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/ggagscdyu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gbcdkhhwq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gghnddhgd.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gggocrecf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/giccyxqbf.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gucvyfpoi.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gudxmjlpw.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gpqwhuwqt.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gmzhbgiws.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gyrcejjgz.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gdxpyffil.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gnmaamzmg.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gufoqwxsk.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gzrdvxprs.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gpgsvyskt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gbatprenm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gfuptwfdu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gzmlwgwfm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gphxptawd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gcgavomsl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/ggacqrxkk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gfjaigiqh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gfoymsdfi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gcpmhejqn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/ghdwiohtw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gqarvoqme.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ghxydfxbv.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gftgvjqzs.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gykmnpdqc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gmyknzsdh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gjxnkxfla.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/giwcptyaq.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gxkcizofc.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gtguhkjml.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gyjqodcgv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/glwzgdbsr.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/givlfzbin.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gfhkzndnv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gndxjladf.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gekarasnf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gkitvqoxt.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gslyxowyj.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gjszpwczl.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gciunxueu.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/ghtifuyld.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gpnhfrdbd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/ggxorrhvw.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gdwmbslfz.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/guydtuwjf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/ggoqkslku.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gbxfdbgbf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmeusuzn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gtzyhgfgs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gmptmqspm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gqgsjoqbi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gzibdyeeh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/godguzvat.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gkzqngegu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gabwmigto.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gdkkyebqn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/ggnccnpqj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gxgzeyuba.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gpgelnzha.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gcgktcmue.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gcghwsnki.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gbsonwavb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gxkherjei.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/ghifouyrg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gpqozshrs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gfygtyqcm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gqbnonyry.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gssojulpy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/ghqcrxqnu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gwxubuzdu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gbollieyq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkftjcep.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gxswkclug.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gunyptquy.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gsqocursw.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gwlhnpnsn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gbyucqamd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gdqbofumd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/glnglhlgz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/goldugfpm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gsnmjtagb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gchyujkvb.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gbdsxkaqd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gmfefmmer.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/glggswudh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gvxjfmhdd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcrjmnuov.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gqeietedj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gxbtmkcic.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gzupigzuh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/glgpwuhht.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/grjfycrog.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gunoseqmz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gqzxcuhgx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gnpucqqmo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/glpawllki.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gvdhyuwyb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gmkbfzghk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gjkdegmsz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gjybdepvu.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gusmkombc.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/giibejgbn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/ghbizcyes.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gwhvkcooa.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gpnyzwzdv.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gkjvjfwno.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gfulsqbst.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gfkydeslj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gnpouumsi.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gnhrojhhw.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/ggybtvsly.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gqddzhphs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/ghhfbqbdb.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gmhhdadjd.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/guempuhvd.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gnmumyncj.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gjbbyvrze.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gvrfezyua.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/ghwedgwpm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gztgoefpj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gepscwenl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/grugsttln.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ghqgwkwyv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gdaddkdvc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/geijjvoee.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gqnmgapjb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/golosebyv.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/glfcxdbvs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsliatrlz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gjipgeypj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjpduitgb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/ghjwblkbm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gdlybsvbs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gvveonoon.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gjkqzcaik.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gsnjvbfls.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsquzpajm.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gpxjvxhfu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gseamkjhu.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gjwrapoul.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gsjujgtus.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grlupkxwq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gycvcfxdo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/genwotdmc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gzejsjcmj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gqwnxpmrp.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtodguxgb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gobddeuwa.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gzpcfqlif.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/grwovbdwb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gkvizynmg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfihgneqz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gmmyumyuf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gaykyksdl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gvjgynaze.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/guhobzaau.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/geqcxnumk.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/giedcybqn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gajtimkte.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gldtecknn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gnutoivqq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/goujvtenz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gaasktweu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/goixozdeu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gimebqvft.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gponcyjdv.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gtejcbote.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gmszfswhu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gzkujbhpd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gebsakbux.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gpnqblrgx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gtufmricc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/griszdghl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gcgnxsqrd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gxprnotjj.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gnanlywqj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gnhecfdxs.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gigndxyxd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcfvklowb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfxblzgeg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gwxpftgfn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gdkjunngs.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbltkaspt.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gacoaumgp.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gkpkprwlo.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaecsoong.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnkztgdqv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/goylhkskk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/graaohvna.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/glbzlazcv.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtimxntep.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzvkmjfna.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ggvdcthnb.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/ggyujkgfx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/godexlbrp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gflrfcfns.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gyzkpmtbs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gluvquqdr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gmcnqvlgp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gjzodjtvk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/ggxrnyipq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/ggemfzxpz.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gfatqroza.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/goxbnmwoh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/ggyhpmrkf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/grtxxfvxw.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/ggwhgrbmy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/ghbdoxkyd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/ggizvinco.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/glmgjkxrf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gmhteoerx.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gxpkoyqjx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpvevnhms.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghsyzdjjd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gswyeddui.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gltshnfbi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gnjosewgz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/ggadjrawh.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gminacdfb.sHtML


<!-- 参考信息 -->