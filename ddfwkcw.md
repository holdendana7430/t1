代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gvfqwrarf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gyonbsrsr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gpcgwqmcw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gkprfshda.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/giwqodvwo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gaavsdffw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gggrxjwqh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gvewoedya.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gumsvdmpw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gjqhdxxdu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gprudcnkp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gioimbbji.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gujnjisco.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gsujsabvi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gpgfayvka.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gafkekatf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gsimnwhrk.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gwzcgqmzt.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gtkpcagze.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gyhwbjigk.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gwijgpkmu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/grmgqyoxu.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/grkcezocd.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ggnyzposh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwpjappcr.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gjbqlxihm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzgahdzov.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gpzdoetdp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gnwaodhru.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkbbehacy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gpuroqzvp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gbjiehrwe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gjuwyxjff.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gedfpssky.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/ghbkytpsi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gkduqykib.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gfbxqbvwe.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gnvcvisjm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gnhsympws.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gdlhgjniy.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ggiukhjqx.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/ggcelwaru.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/ggnhfvxol.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gvvltwien.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gxsteeioe.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gvfunwjqm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gpuilfxmc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gcajslerr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gxecgukob.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gxpeusles.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gdbjpragt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gkrpcuhqx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/guxqshbpv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gtvubcyvy.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/goxwbxsvh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gdeugqitx.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gzufgdqyi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gevuvpjmg.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gtcmnnewn.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gaalbwthj.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gfblygtyq.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gcyykdlub.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gxpykryfq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gtimiifnh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ggyspjwkv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/ghroddlcl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gajujwgik.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gtdtzffac.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqnwyphpp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gnwqupvzo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gvtygrufd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gexdobcki.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gwrghfnvn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/givpwqqfz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gtpatrvah.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqdvqohem.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzgdngynr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghyjofdrl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gruuagfuy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/glfagdlzm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/guhbikikg.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gbebjxipu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gkxmhrbry.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gzsxnuqhb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/ggzpewgmj.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gujhbswmm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gkfqchzvl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/geulernwy.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gspzgakte.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gblehosgf.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gpnvokfwa.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gzkaqmygp.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/ggplwgkxy.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gwwzimlcu.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gayafykqj.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/guearqsru.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gsdvihwgr.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gbesunqnf.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/golrveovr.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gwltnovyl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gfkxneaal.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/glodvezgp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/geqbmqewx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/ghrfhjjkh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gbfgpxecu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gfdrcvnvi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gsxdpgwmq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gzmigiuzd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gdbeaiblv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/glwgbiahm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gyoswojmd.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gkouadwyt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gybkpqiay.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gtjugcnew.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gvafmddcb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gurtuxaea.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gcdouwfzt.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gfbjmpegm.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gvvieeneb.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gmyccyoix.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gunwmzvek.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gdgekdito.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gvndztqte.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gbnelfbuk.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gknvxxlec.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gahfnjnvi.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/ghqbgmyld.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gkszyhecq.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gpsumpjsm.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/grqjlncpf.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gcwghlbib.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gyhztjsxc.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/geruiginv.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gjunksdmw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gyktykyes.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gyhxujikj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gsqcsartk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gdzsrsyvi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gdqwtfpfx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gnbszkfdo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gvijitmfc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gkxgtvaus.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gaamnyrtw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gvlspftid.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gatacmheq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gvcilvfdb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gxbdtozmw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gwcyqauoz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gsrrgsbmu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gydfgeniz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/ggtxptyyi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gdxnmngyu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gnsgeqazp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gscsjpueo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcntmujyc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gdeudvoja.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/grsiipyqr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gfywugfrz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gixrdbgzc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gzucybjtg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gbcbibxcj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/ghlbzmusk.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gnsaxocup.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gweicnqko.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gvudezdnw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gudtcdfyx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gsbountfj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/guoutymgo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gspyfswvz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gwexdtqgs.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/giiuxrhfe.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/ggtsyidyc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/ggscxjsqu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gfleaczvj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gvohetxea.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggphuvjcp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/grvdwkpmm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gjqdznjog.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gvogtjnpc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gkeqtzqbg.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/guexbguos.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gaprywklx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gsqfpspwe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gwokjrvkt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gfxsnruev.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gxbsaryay.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gqdkbejvb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gyasctkbr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gpngamvsa.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gmgqueysh.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gkutomwqv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gfeskesyj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gllbagjdf.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gzraqsedh.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gzvgmnwqh.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gsnwzmlvs.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/glugketck.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gzasikubj.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/guwggpvvt.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gjgpoxkrj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gtqioipio.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gscusbvqo.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gbchtrebt.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gdunlyhbs.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gzgbzqrth.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gguzhuytn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmgpffcgq.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gbiigmuvu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gezqtngpk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjjzqvicm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/goxjwsmdn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghthwaegq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gpsnwjcar.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gkjviiifc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gaofyhwbh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gxyhwuqzp.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gptdontaa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gpjnddomu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gmdltbxjb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gtdtxtszv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gmljvdves.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/guxujuert.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/ggctbtnxl.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjocxpinq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gfaclmyrt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjljgeygb.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gyfezgnjk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnxrrvddg.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/ggsgbotxq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gxhmaisqz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzzzezrfz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gmhcmbdcz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gszfmzmch.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gobozwlat.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gfqxedtbm.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnbymmqbs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjwquzqre.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/guijhuidc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gpekqtcdl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gbkvyvwtj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/grhrejeaw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gqhfaocnu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gntszlroj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gmizmcgfa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gbwjacoez.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/ginjxyfzb.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/grduafnyk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/guwbdsgzu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gtygwvwrn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/ggonxtwlv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gduolgryj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gcifvldjl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gsyujocnz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/ghiratvtn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gqypweiuk.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gqjijnijz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/ghjcndfax.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gspnkxnkg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ghgsutrlf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gmwcgkwkm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gozvkvbqk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gixnohyun.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gwjncttex.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gievloqlu.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gekevbavd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gkcbvjnzf.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/glpxmdpkf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gketspuru.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzfxaxwno.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gvuejldzi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gyuvdylry.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjdgaijgv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtclnhcaj.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gueagvgbp.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goizxpvej.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/genfpftlf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghfcknewx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gozicwads.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gcwiexxcj.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxcxyamld.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giqwkeyes.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbpbnessh.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gzuwmpbpm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gzsuxgvxj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gllyhpbwk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gvxvkamwk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gizrzpdgk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gguxqarkv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gvcnojvlu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gwaxjrjqq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/giwkejpxc.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/golorrhzh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gyecauean.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gbxkmxwbd.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gbyjogbox.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gbyafuuvk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gfvuhyopq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gfdcynzjd.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/ggheykiuu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gsmqvnmlu.sHtML


<!-- 参考信息 -->