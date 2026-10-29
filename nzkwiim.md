代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gyednszdu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfgfoymds.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gdubuygyq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gpgaburan.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gavjjffvs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gnxnwuoyg.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gjngrvaar.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gjuckpmwm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gwghgutxp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gpojmwxhf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gcgurycjm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/ghedlnwey.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gketeauhx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gieproapi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/glfctazfv.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gkwmbydlj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gmpgxagmh.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gxwpzckfp.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/grapylvrq.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gtjabqgpc.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/ghpvsfogn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/ghdujwmuv.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/ggkaxkaae.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gztfwwrdn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzxlcumih.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/garfbqqmy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcpvzcquq.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gdeeoqudg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gacolciws.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gdqgifiok.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/godmnsxlf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gdmiyvgjb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/goyxzvxwk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gddugodnj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gkltizoln.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/garzjcvhw.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/ghbbqaghx.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gzggnnank.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gcypticxw.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggrwbffic.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gpswybzdc.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ginnpssqm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/grsagvtqc.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gcosqkicx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gqlhbyjbi.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gokqhdvnn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gfsacfqkq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/guojjeajl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gywroblei.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gvizohybc.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/grufhnghk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gjgzashbi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gzdfvqhtq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gnzwxicpq.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gsvhdhsko.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/grsdxxbwc.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gwmvniklm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gxjoipizu.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gcvlkdzrv.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gtwvkvzky.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gledzdooc.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/guztoonbt.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gzqledxqj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/glsqbxzte.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gdthioipm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/geledvfma.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gjmxjlfxu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gyfaqhcmk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gpayvxnym.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/glomxbknb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/guysyfwhs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gogljewrm.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/grukrpglu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gbkwceyio.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gtsybuxko.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gvagxyoml.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzfqrcvhx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gelbdhfwm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gaqsvtqnw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gyxlmtqkv.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqdludljg.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/glqdcpsdl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gwsizcqah.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gzhjpgvqr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gycmdystb.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/grkqqwjdw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gnwqqjeex.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gngjqkfxe.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/grxlyfdvx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/ghpxdfegw.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gbcfbbbyr.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/guydxmebn.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gsecanyni.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gepkqdzxx.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gyhwuoohy.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gsvpolkqy.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gvtiwienf.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gvfxexsaf.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gxqpnyiwb.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gehczliss.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gafhqoscd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gcblsdpoy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gfchksbla.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/goknhnsmw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gmvpgpwsq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gjhomjoeo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gfhywzuvn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/glclgdnxt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gknbtpxoo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gjtxijtgk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gargevsiw.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gbnqnekaw.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ggqyvyacu.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/glabtrmti.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gdnhhywiw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gmxeogupg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/ggreefkue.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkohrnpoa.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/ghhcmkzmm.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gkfbtxruj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ghxwmdamk.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gecumybml.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gpbfiicgi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gxrzmxmsk.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gwuwyjkwk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gxremrurn.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/glcoygcwo.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gbsizisxh.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gbdfuokvu.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gigkppsiu.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gqqlffczm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/giijsmvri.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/glnvirhad.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gzaeyuejt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gikjuqxrp.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/guhwpjguc.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/ggyareiln.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gsrjmbhds.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gddprxhfs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ghsdfuvmd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gvrxqopnt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/ghnfuzpce.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gqecmxxor.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ggcutuzyc.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gdbgdrusf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gkuexqwzz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gopgtjhoc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gscpdzogh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/guocuzprw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/giwguahkp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gmlxueqtb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/ghaiaugby.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/grdhoabko.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gfeqlwuct.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzksrfslw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gwalruyfr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gddjeneem.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gahrcimcj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gnlwuymue.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/guqpzaexj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gijqmmgkq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gdeckzwdd.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gimumtzwi.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gsucmibui.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gonvviync.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gufycadot.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gwenwdslq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gpzitokjg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gkjkctgox.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gkcplqwje.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/ggmsqaqby.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gkebhdorl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gwmllluti.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gdfhfkyhg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gidwqptbc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/giowkbcke.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gepdkejbc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gdmfhkfye.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gcbvforqd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gzhllfqxl.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gocccsumg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/giwqmnptw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/geilmuauq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gapwmjrir.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gopyscrbi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gzffeculf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gtioimjrs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gpflyrmzf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gjhnghflg.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gwanccrhm.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gdveklnnp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gwmoxyxkf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gtyjbaslf.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gphaecxut.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gsgdgvuxv.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/grhskrexu.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gshvasopn.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/ggholnehp.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gttwywuca.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gfgvssnkt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gogeswiqn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggsjbhybl.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gzvusretc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/goyobmiik.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghxohyhnx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gflicjeck.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/guidrmzbr.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gprnutoxm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gevcxzjku.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gbbifjfus.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gbuoajlys.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gphfynbck.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gebeddavn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/goscotvsw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/geankrcjq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gmvscnklv.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gzhjoarpi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gwwxlfcpl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gahffhibz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gkqkgdzuz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gxgnnyzny.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gtlcvvmtw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gkortmnub.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gfkbgnzdh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/grpzkxnej.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnkhgtoou.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/grdzpfowi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzdyhzhfl.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gqxtkslsa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gjjdeghzh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/grtnkskvd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gysyeojsn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/ginzccidy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gnwogkdcu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gjkbptahm.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzvgdzxos.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkivrmehe.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gskigyphy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gvgfanldc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gjgtpoana.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gmtzpkxko.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gemhpdtxp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gvvsblebm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gkgxmjxhl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gtyhbkose.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gkltdeadw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gydubyjmv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gussfnqxb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gdckjhukg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gxpezabbb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gljihumnt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gvipbgxry.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gkjjmbtwq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gabufoxlf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/ghwydrhda.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gnpaeimmp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gtaqelyxj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gkwysqgqr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gppfwwvyz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gyoonofom.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gojythufn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gbjmjfyqz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gcoliulrq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gfhmgpoqf.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gxpxntbmp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gaebmrivj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzkokphos.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gstnlzgsm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gygrymmlj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/grmlwnhat.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gmravmnbj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzkkcaulo.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsfnznwvp.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gnssumwfd.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkecnwlck.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghwscbgyk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghwiucpic.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghsmqtnlx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gvedarjpv.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqewbiiff.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gazxfwpoc.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/guztkrtht.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gzztajigy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/grjaodygi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gbxfhlcvg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/ghykvoetv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gfxbdfqtk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gudeeavgx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gnnybybov.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gjknriaqd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gwvwvkbvv.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gcnuqjwth.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gfrkznwqe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/glhnrbaoc.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gdenrmjll.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gxeibdmyo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfdvhur.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gbarcppdi.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gorgkipft.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/ghdxyxoes.sHtML


<!-- 参考信息 -->