代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwsuoehk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhjrjoeu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fanxiaobao.xyz/Article/details/gkrqfevil.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkemlbit.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fanxiaobao.xyz/Article/details/gwlajxlcc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjtckrqc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkonqgyuz.sHtML

[D26] 数组转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gelkapqbj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvxbigor.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpejbwwn.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdjaotsu.sHtML

TS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfswucko.sHtML

Java: String.join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/ghrygrvaq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkmgeugq.sHtML

Ruby: arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gwpjqkffn.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrptukxs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsthmglcp.sHtML

E. 字符串处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gcexfkhdh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzlkwneo.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagzqjaro.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwymcfto.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fanxiaobao.xyz/Article/details/grjsbqrrx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrkekqix.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fanxiaobao.xyz/Article/details/ggzniisge.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzdwpstj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuvnoxvd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fanxiaobao.xyz/Article/details/gvakornwf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/giyjbsnrl.sHtML

[E02] 重复字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/golarulxr.sHtML

Py:   "ab" * 3
来源：http://3g.fanxiaobao.xyz/Article/details/gwslqawjx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gdqguhmnr.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gluvhsztm.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gpgysvopy.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxsaqqpi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gbvdhdzmh.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpujbkmd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/goaqbgpqg.sHtML

[E03] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gcozoeymp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwuuugzv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gmurnvkra.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/glpdshynu.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gdnvbqejz.sHtML

Java: s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/ghaegztsl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqyrtgwj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fanxiaobao.xyz/Article/details/glesfssij.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwqmvwgt.sHtML

[E04] 查找子串位置
来源：http://3g.fanxiaobao.xyz/Article/details/gduryidev.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gnqkofpzz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhdbehpx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fanxiaobao.xyz/Article/details/gomwhdggo.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyhkazlm.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwiqwcgu.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fanxiaobao.xyz/Article/details/gqeuedhte.sHtML

Ruby: s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcametijm.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdszrnuvw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gvysimwle.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrhzmsku.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscklpxxd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/ggvrxkwxr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhfdqfqu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gljlavyzo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fanxiaobao.xyz/Article/details/guamrcwog.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkzzozaa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjytmpsav.sHtML

[E06] 替换子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkcvbapc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnhzxpozn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gqvoqnmyd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnencbsan.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gtghxfbdb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmktxmqaz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvmwwwlm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gyeleears.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gnjvgaadu.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfprbusx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupfbbgop.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzbxebzg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gxwuwyrqb.sHtML

TS:   s.split(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gyzufxxgg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmetfhti.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmjkwtls.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fanxiaobao.xyz/Article/details/geqfuiqbz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fanxiaobao.xyz/Article/details/gupyrslnn.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjojbcols.sHtML

Py:   ",".join(items)
来源：http://3g.fanxiaobao.xyz/Article/details/ggsijeboh.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcosqksij.sHtML

JS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gzuvobzhm.sHtML

TS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gzuwzimmu.sHtML

Java: String.join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gghpdltux.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fanxiaobao.xyz/Article/details/grlrktacz.sHtML

Ruby: items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbipjfsim.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghodojrjw.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garivsceg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefhescet.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/ghtfihamx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzkwwleb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgsyevfq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goggwyezn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fanxiaobao.xyz/Article/details/glvwzsfwr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbzsbuml.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fanxiaobao.xyz/Article/details/gkyrztlqu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fanxiaobao.xyz/Article/details/gxhxrtpid.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gkpybflsr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fanxiaobao.xyz/Article/details/gbjobrfrz.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gppiwbefz.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/geguqevwk.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gqnzakxub.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjdrmtzx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtuhlvos.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fanxiaobao.xyz/Article/details/ghjkvzker.sHtML

[E11] 反转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvdxggpv.sHtML

Py:   s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/gsvllvghy.sHtML

PHP:  strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gblxrvrcw.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gbflotgte.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdgdtvcz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeicnuiv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/ggfrhhnuu.sHtML

Ruby: s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqdnadrs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gozyjrsqv.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbryywfky.sHtML

Py:   s.count("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gvkcfekuc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fanxiaobao.xyz/Article/details/gclklebet.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fanxiaobao.xyz/Article/details/gzefuvrhe.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/goqzqfmxz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgkqzomm.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fanxiaobao.xyz/Article/details/gwsjzavct.sHtML

Ruby: s.count("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gfcsfugcn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fanxiaobao.xyz/Article/details/gtaorsrek.sHtML

[E13] 逐字符遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdwuoafa.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fanxiaobao.xyz/Article/details/gsensvipa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkwzrojg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyjsvbgr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gsshmossv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkedansyi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdksmrczw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fanxiaobao.xyz/Article/details/gqscwinvf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnfqoysz.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fanxiaobao.xyz/Article/details/gpoduzjkw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkfdmoer.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfntubnj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/gcdkxruhb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceqfqbgg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvstaidq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqeoktkd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fanxiaobao.xyz/Article/details/gmgajyfjy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkijdqlwk.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fanxiaobao.xyz/Article/details/gueqotmnb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fanxiaobao.xyz/Article/details/grjqbpakh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gjnxcocxi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwrubdjtt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gacbpcnmn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fanxiaobao.xyz/Article/details/geptwhcmt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatltdlic.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyclmuci.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fanxiaobao.xyz/Article/details/grypklktx.sHtML

[E16] 数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsoxvhbe.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnwiwosbz.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjzkitmg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwtfmzfr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/gclopfcgl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnojaqyy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fanxiaobao.xyz/Article/details/glkcblljk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gtjvbnzwo.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gguzfwavg.sHtML

[E17] 首字母大写
来源：http://read.share.fanxiaobao.xyz/Article/details/gclahrlmm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqisyodvb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbnofspy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhtlcvho.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxcqedioz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fanxiaobao.xyz/Article/details/ginueqivt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbloncxr.sHtML

Ruby: s.capitalize
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfweojfg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fanxiaobao.xyz/Article/details/guvfauosm.sHtML

[E18] 模板占位符替换
来源：http://blog.fanxiaobao.xyz/Article/details/gehbozzpa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsbsivfm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoxcavba.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdsucpjz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/godzqnjlb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gpfrebvwg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/glsjrtlah.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsqmyokhk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmnczwoe.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeutgkbq.sHtML

Py:   s.splitlines()
来源：http://3g.fanxiaobao.xyz/Article/details/gnakyxdbw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/ghgnqpphk.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fanxiaobao.xyz/Article/details/gqpbhibmb.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/ghvjbjqio.sHtML

Java: s.lines().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjicmajrb.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeqjcmub.sHtML

Ruby: s.lines
来源：http://3g.fanxiaobao.xyz/Article/details/gwelavlqe.sHtML

C#:   s.Split('\n')
来源：http://wap.fanxiaobao.xyz/Article/details/gythkaxcs.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxolkbaiq.sHtML

Py:   if not s:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpcvplcf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjkfabcr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzvkhfjau.sHtML

TS:   if (s === "") {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gunijqidj.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/geacalmah.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmvipise.sHtML

Ruby: if s.empty?
来源：http://www.share.fanxiaobao.xyz/Article/details/gerebuoyk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtewqbpbx.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzviyzhz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrxjdyxs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqcudzgk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gmmuuvvks.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gsddoslmb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gsgpnpiix.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhsrnecw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryrartyq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gfssnwuny.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrvhfldb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gyeluhxbh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkiaqrco.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstqohkha.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/ghjtwgtpe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzumbahr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fanxiaobao.xyz/Article/details/gbzjovkcm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptlqpmwy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gralobmpu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gufqrttlu.sHtML

F. 文件与目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiotrngc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqbeqwlrl.sHtML

[F01] 读取整个文件
来源：http://wap.fanxiaobao.xyz/Article/details/geatelqdr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaelcdnmw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxakymydu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fanxiaobao.xyz/Article/details/gihnnaxfr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gtenzcpbj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gewogtdjg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fanxiaobao.xyz/Article/details/grewntqcg.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gpjvvxtuz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrxrigsh.sHtML

[F02] 逐行读取文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjesyjumm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fanxiaobao.xyz/Article/details/grkjkeujt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwjqlpaak.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzdaksete.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/glnttiurs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gaqyrekvk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxpkkrgl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuvxxwor.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkycrxocb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdztexyxg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fanxiaobao.xyz/Article/details/genudvgak.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmttoexxa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/ghaadhzre.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskbofgkh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gmkainpye.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fanxiaobao.xyz/Article/details/glqzlwhsn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/glbjkjwkl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdczzuocg.sHtML

[F04] 追加写入文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyzydwmv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwpjecst.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fanxiaobao.xyz/Article/details/gftuplqdk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/ggyksstry.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gfoevsuiv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fanxiaobao.xyz/Article/details/grgeitznr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gpcthqqiq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fanxiaobao.xyz/Article/details/gibisetiu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gmcsxmkyq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gyudokeoo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiylblqw.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgwvcsuq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gtgqkstfb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gycjmmspk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gaziqixzw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzrhwdpy.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaivaukdt.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/guqeknyri.sHtML

[F06] 删除文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzysjzgap.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gfuayzpyc.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnbigozo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gucskgsyk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpbgnhuo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvbkljom.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqurvylg.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtqigmtd.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsarxtvz.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/gvxktkydw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gsrudtrsa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gmfmmsicj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gptxyxgvt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/goxhjyiek.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fanxiaobao.xyz/Article/details/gxjebbupm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcgmpjyo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvvmbaah.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqahhypxq.sHtML

[F08] 遍历目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gvivbjpft.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzryvnvp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fanxiaobao.xyz/Article/details/gonqlyxbg.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrdicgiy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiqaubmw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgzwndfb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gnptknvum.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/grbvidxyp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzfwyzhj.sHtML

[F09] 获取文件大小
来源：http://baike.fanxiaobao.xyz/Article/details/gktturqhb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gearxgwfl.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqmjvist.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gofaccpne.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gfenmqjgq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gwoslptet.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypnslzyi.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyudoopdl.sHtML


<!-- 参考信息 -->