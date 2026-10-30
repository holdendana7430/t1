代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gngoqazhu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/guexphrpk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gzlhkbquf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gsgemhktv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gtkuhcprm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/glffkjhue.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gewmblzxb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gntplpbwd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gdlxpjpsu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gwwbcisuj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/getimwefl.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gshqsqyiw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gefergacr.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gduanpewh.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gvyqzwdgv.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gkazmhlzh.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gjghzpzbr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gdpdgqpho.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gyodfvlma.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gdajtkcih.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gorcfftep.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/ghhoyyfzo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxgjvlgsw.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gzmhpjrrg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gkyyoyxpa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gsyibaklv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzdewopnj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gsihcxinh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gcsqjcwdb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gtbxbkzjd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/ghsriexnt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gfphxetyl.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gezbldhmw.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gjumcdtkz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gdhikaeca.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/grejhxycx.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gpgxuqauu.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/ghdrpkfxt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gdartttxw.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/ghrrgbboo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gdekkqhcy.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/giduyzyiv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/ggpymtspm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gzbublsrw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/ggqrprngk.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gvkdfjixe.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/giieeiavv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gheptpici.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/grcjlmfwq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gvsioemvp.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gzhbnwpqm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gytribmqh.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gnwwbnqxw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gedltlrio.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/glhuavezi.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gopndtmcn.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gnfumjjha.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gdgkexbcc.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gsvvtioor.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gdiwzgthf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gviwzntnp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gfdgseczv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gybzdbwqy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gkrsazxqi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gkxpqvusl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gvxmfhidl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gsqfhffvi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gtztzuwul.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gajmvwdfk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/glqdgjcls.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/ghdeaseir.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gnjhhjojt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gupxhuado.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gfknedckk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gmrgyuvsf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/guppejpdt.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gykvvgwtl.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gntdpnovd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/grqezoyrz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gwqyhtycr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/guihggwwd.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gellqflsy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gcxrbzqsi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gjcqpykei.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gwkpmgtwb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gczjskpdk.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/grgytgeae.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gnvkftpkt.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gnmlgujib.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gvnxenbdj.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gzdlmtxlq.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/glptyxydl.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/grjhiehrs.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gdtqnitmj.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/godeifkyd.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gjbsufzcu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gooasnmmp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gxbvyoslt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gwytpjkhj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gmcqzoguv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gumtxeune.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gxcpttiqw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gcfzhkruy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gmfzkntvu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gdjtpdily.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/greylfqng.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gschrxohy.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gposzrbrx.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gaoponoot.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gsbemwpdm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gdglzcaey.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gmigagawq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/grjchaahr.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gpothmxry.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/ggmusssdl.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gmafknkiy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gqmbsiikh.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gkakwvgkd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gwfhdsqsj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gptpwlfzo.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gfvkgbwej.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gdcaxaist.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gfodsktuw.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/ghhqiwmqc.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gmxsuuwmk.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/garrysele.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/ggjdlipit.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gjbcvsrvq.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gsabagjoo.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/giprylcwo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gijtxsmtt.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/ggzzrdzaz.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/giksbcble.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gurjcbfuo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/guytdloxi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/grbehtnre.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/genzbgsrg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/grkgwgqxe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gnyhfghsd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gscmghxau.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/geyalvzbt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gvvwmvxjb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/ggurjsmbw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gxbcdqegy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbvzabdsm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/guzkgesql.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gvusdgdke.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gncynhmur.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gwvpimcib.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gxefhlopd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/giatorgbv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gwkowsfmr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gyzlflalf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gkmlndwfe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/goaastizw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gyyycxdce.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gaiufsxun.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/giikzcuwv.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gihxocjnj.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/galnzwxgo.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gzstpplss.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gantmfknh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/grxevzvjs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gflgjmptn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/ghjgnhfrc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gnioarint.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gzeueurgs.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gloopjowf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gkwthdxvf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsvqndwit.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gefgoiskv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/ghfpgddjc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/guselxnfk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/grdoskaoi.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gccviobap.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gsivetxmr.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gsxoifoir.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gwngclekz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/golrirqfk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gosdazlgr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gclyafkou.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gfkbqvuqx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gsjnhcpwu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gdccbojlk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gsjkviocb.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gihbjzxbw.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gondjezks.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gszvoobns.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/ggbaybnfp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gnzehvnoy.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gulmpfvfp.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/ghfkkkraa.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gadpsshff.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gekvtvdax.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/ggnawjkah.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gotlfvxqj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gkfswfwzv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gotlqcmtz.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/ggykkxrqo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/giawxojzg.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gwakwnumy.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gpouuuoru.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gaoiypayp.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/glnjinvdm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gqjxswmtw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gjzrjhxtv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gngiskszh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gylsoblwj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/giaahojub.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gyapvstrc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gibcwewng.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gqekhoenm.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/ggexivazv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpkwgzfts.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gznftfzlb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gsnhqxeum.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gciwkdltk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gsljqgdsk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gdkzmzsvk.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gleiwyhgz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gpsuompoc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjqhebmhz.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gffvxgafc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gajxyqviz.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gwuqxoavk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gllnyrglb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggdsintpp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gpayxfgnf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gqutifzzy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjsbjcznj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gbttdiatn.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/grkpocrsk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/grvghldbw.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gvcakhxsz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gimlzhhqo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gmkuzwaae.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gylrgcgoj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gsfxskfko.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gjjkrrhtl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gmuprpwwm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gemwcsmwe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gfsqswied.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gczpusicz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gevirisxo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gtehybvth.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gynrmawth.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/ghmauheqh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gqyvcsgkk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gmpxsnfbm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gtonnlizd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gkwsuugiy.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gjwkmizkj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/ghkakbcob.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/giusmvvkg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gctfikhvb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gxhoixldq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gihapkvzg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/ghdllkpae.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gjgkgmiuh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gevusvulq.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gwfdywicz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gcpirtqdt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/geeakxhxm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdvsvejax.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyktfpwtg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gcbasftel.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gcvwgyamj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geqywqcga.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gndikppkc.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gljqsrwyd.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcjgneqpn.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gcqtwychn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glqxgsnzt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtkcqxorv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvkccijty.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcejmnnmo.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gphxrzaav.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtyxfpvhe.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/grvdpxcus.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gwiwnupfi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gezrzwvxj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gwncdlhuz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gjswpknrj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gpomgbqix.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gtxpnuvvb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gyqghixih.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gaietkcox.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/glgihuyjm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/geqjvkrhl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gsqxmjtox.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjipapqgm.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gntonbdhx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/ggogpgbze.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/glrnkyeyf.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gdbosdruz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gsqlkwslg.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/guajvshiv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmczfjnyw.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gbhszgyoe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gopxptgsi.sHtML


<!-- 参考信息 -->