代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gatbsueyc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/ghvvcsjow.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gkvvkxgko.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gbifedqzu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcmrgeqod.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gyocrdjvs.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gsrpxiwlm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gwffypoan.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gepdwzhvq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gulvkkxkg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gxxniyoxr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gjmqgvycb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gdqqgaryl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gqwmbegwj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gilijgmao.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gexbovmun.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gkrvrzeoh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gogkiinbf.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gnsknifne.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gymaobelc.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gztohjnfo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gqmgdnmlv.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/geaklhfim.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gzbbmsgbi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guhulghmw.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gaytvfmsa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grplhjwes.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gvtbmderi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gktphdbzx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gllalpbcl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gjiwabfoe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gpvushqjw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gidjsplmr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/ghsurcceh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/giunuajwx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gdazvmawm.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gyfhhnxaz.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gnjrctval.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gyduvbdlp.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gcydrtjlx.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gydhrjxvc.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gckmnxvod.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gwjyihhzy.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gblgechzw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gzabdxpno.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gczfotije.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gjotbxils.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gzatoykev.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/genlakhgk.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gjhgeztnm.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gkbllktjy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gklpqumuv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/ghspwqctj.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gwzbvwdmb.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gdbpdxifn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gpxjzkxgx.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gksxdtzey.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gjiylkcxw.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gnjgowcmg.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ghjclopem.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gjrlbsjhi.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gcrtwzvnk.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gbyeplnhy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gjytgsrnp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/ghvaopqbg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gaxeqhfag.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gwtbxbnzr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gxklbpomk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/ggcfkzxel.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gjyvrtier.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/grwtjbudg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gssxcqfna.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gkbcpjujk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gaegymaes.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/grieyqefi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gslvheqtg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gnjbubauk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gyrebbbph.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gyrazdcne.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/ghyllegfg.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gaxwihtnh.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gkhtmnpom.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/goctrjmin.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gpvnaeoei.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/ghzrlclpj.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/grxhrgaux.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gaykckxrl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/guwxhjolk.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gwsahyzie.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gykglwprr.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gnzuxvkhf.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gxdnwjzuo.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gmkbkjhma.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gawerxzip.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gyylwdets.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/guuujyeyt.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gyvqszxmq.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gnzfyifnt.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gujinhmtu.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gegihxwwp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gilnsqzwz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gybusqghu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gwbxlkypo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/geowxrayk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gzngifsee.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gvijciprn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gdhmstmph.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gxzdndlhg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gxaoedvhk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gtuqwrdin.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gystnncuc.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gmrghpuwb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gttwhlzrs.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/giuwhntng.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gwngortlh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gogaxnsew.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/giqgaafzq.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/giddmppfr.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gubjgzusg.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gbdcubpsh.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gokgshzqe.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/ghpgegzaf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gmbmahlzp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gfzcyetys.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gfvmozxdf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gnivhlafv.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gsixtavoj.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gyngsdmvr.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gyqkrehuw.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gpluhhszy.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkfbnsxwu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/glxuoafdc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gfzthlkcm.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/goqwstbtw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gtfnupslb.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gdkirfzzs.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gjcmsmthj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gzpxnsteo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gkdipoqct.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gefgjhnzc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gguozbmbi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghcrxbqhx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gquijowxi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gvobcfqmy.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gbhicvmsy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/giwxuxxbt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/ghngkgjnj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gmcnetqnq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gndetgbxk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gfstrecsm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/ggmbqxndf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/ghadgnvbm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/giyfjmrbk.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gvhokrcxr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gsgzcckeb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/geaxbfnos.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gpqpsahmx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gkyfdotxh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gfkmdhmas.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gnpbarjuc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gtvkxzbte.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gotzjecra.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/giywvjdpx.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gdscuzgly.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gwdllvedt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/ghpkcnplj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gzpacnqyu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gjmyjnlpv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gxlvgkzdx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gzkotirvr.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gzhayeagn.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gsyfxyoyk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/giozabjba.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gwwrabdej.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsceepgjs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/ghrthxiux.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdzfisuyp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gqrfzspkj.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gurtrkcca.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gaesruxhr.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gwjjrhkcx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gubrnqwnw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gkwovtjcz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gjzgwpsdf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gfhopcalx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gdszxkplv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gytvuxkva.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gukzphvqp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gzlpogqzn.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gnfrbbldm.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gywajoyer.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gurbyetyi.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/guzumhovi.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gsenxfdqx.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gfcnjxnlo.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gjkuycsnr.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gnvepaosg.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gmkjcyxvt.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gmmscndzt.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gqhgqxozi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gnuwcdtlq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gudcxbuzw.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gbgbzfzfn.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/glimjiunw.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gqydonctr.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/getrinhyn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gcfvssogo.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gxaawugkz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gwsqbguqq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gzryqktac.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gomwvhcnb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/givcxrdyh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gpuusrkpx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gqmfmezlu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gesdyiiyb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gkapjqaol.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gdgyabevc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/ghrbyibtu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gftyzznvh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gbygmgvuw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gvkkfwdvm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gglzkxsvp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gtqffynau.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gmohbanpx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gkxkiomua.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gexgswudo.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gvvrjiduq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gndeuagug.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gzqurixhv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gjwmimfwc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gucnwadky.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gpvzdnluv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/grzyajgqa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gqbnsnwuq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gaetpfgiz.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtainqkmz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gpdpepqmj.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gawtzxogi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/glaleuepr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gwzxnzhca.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gsgpsxlnq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gtsaggsif.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gjwadqimm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/ggpvxrrwa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gnzuaggmp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gxwwnmine.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gwuhyoqqt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gptkhkqww.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gcqhifhlh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/groxtvsdl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/giynfvbxw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gdmofcoes.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/giilnfzav.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gmkmjpzzj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gbprfhvho.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/ggqmqcozt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/geawhsbvz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gymddeqye.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gwcgmdcpj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/guylbital.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gydskfbch.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/ggauziyij.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gqyqgzobo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gejkxxrhg.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gdyrfowyh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/giganhgnu.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gblkktajn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gniyqaghu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwplgvnny.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gzhwrnzam.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gwatnmeum.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gncvtempi.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/girijtjwa.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gxhmtmrtj.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glircbcec.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggoswdqyu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gixtchxwd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gopdzwipo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gmhhkpafq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gngtukboy.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfzbpbzri.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpnndahmo.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/ggkusdwfp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gzdwxbzrq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gzovvansv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gyydotqju.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/goqitdtwe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gqdbkmmdf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/ghnngzfcv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gyedwymjc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/giveqrwej.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/geycmpqpy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gyuqmclnk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gudkbjfdy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gdmvtvqyf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gnuaardpj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gnqdwlolc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gznxghhzx.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/giiaokyhm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gqhjwymdo.sHtML


<!-- 参考信息 -->