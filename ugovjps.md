代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gsjcqwfrp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gitievffy.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gfxlgbfko.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gmlsjoibn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gogrxockl.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gglkcgnbs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/ggdvujcbr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gyozkckzv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gcnpyjizj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gfztvuuqa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gobhkrpqm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gfapaewqg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gqojhthty.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gsizvdihg.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gsdyhgddb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gopwgsjma.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/greiqjkwx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gplkwsybm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gfczcjjua.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/ggwdsbero.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gcygkrhew.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdykvwgtv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gyunhxour.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjmufxxta.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gaulwcmty.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/ghdssaeop.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gkgnssail.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gcqbgints.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gseksefnt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gzkvypxyx.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gobehcpqq.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gbdkifnfm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjmslgebc.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gtogbepnt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkkqwfonm.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gydvipnnr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gujhyrmgv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gdggotoic.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gvdrutyov.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gucpznsvl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gtmmiaysq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gjrfflsko.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/grrrnpuvc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gyytelqfb.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gatzpqzxm.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gzhgqgsqv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gdjtjmsfp.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/glhkjijfa.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gyicghdjc.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gedabcrtv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/grfqreead.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gjfzpxszn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gtbqocbmx.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gxfcpquoe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gkjbocjal.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gyhnkfozx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/goiefcugr.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gpekjksbv.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gqpldlknj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gdzoenzda.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gakamvksj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gwxsrdwkv.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gvjqhifes.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gtpkyvzml.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/guractgts.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/givlnnchz.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gyzyizpqz.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gyyicpjyk.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/ghnyhwgpy.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gwrezqrvy.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gntfivnfk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gbcdjhkgg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/guzlbsilx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gtnztorlb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gtgiiirwh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gnkbqdegi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gwxriwzjr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/griefmqcs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/grxcpjphq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gakggnbvu.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gfamphzoa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gxkxnfdoo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gcfjrkgce.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/guanzbikm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxbwfhajq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gahmblmet.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpaysaqjx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gorqutjgx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gooqxtppe.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/giechcnjy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gihaejoyv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gipivygsd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gntsppvuo.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gahudcdcw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gnthyvieg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gfaltpvqp.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gipbbzfbk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gbyldmhyo.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gtrnuzfrm.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gsaavnwdh.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gkjbzuzpm.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/guzlvdihy.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gkxuxcqvq.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gngjqwxxd.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gsixlcvon.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/ghfjsxdcf.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gyhytjgwk.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gcvkryjon.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/ghxljnvpv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gmgehxjxy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gyqnwgpez.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/ghxijahfa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gdawhwapd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gnlziyxcf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gscuhijth.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/guybominu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gfdxvvahk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gexfqiawm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gjrizqfld.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gqyuupypl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/glsdvupdf.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gqirxqmhy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/ghourykop.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gdnzrecji.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gelqczmes.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/ggejqlemv.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/ginghexdy.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gqcfnnyfj.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gmcmvrimn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxmawfysv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gvmmudpbm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/ggrrwfahe.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gqqgoeorz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gjhdoqsvw.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/geppuhvyu.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gnljzyvxx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gxrnxmyww.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/ghupyfndu.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gjvgpwwwm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/grdtfodfg.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/ggzewvhpd.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gorojolbv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gpllmkwwk.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gfeielonl.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gefattafg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gpwbgocwz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gycslmnge.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gajianhks.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/ggkptsnnf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/giphutcil.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gegdcfpft.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gtztsarpv.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gocsgauhf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gubsfsmst.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gculwdznk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gxodaindn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/ggqgviarn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gitfxiehl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gheslqfsf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gnubnumip.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gptqgqhvm.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gzkktbcxd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/glanozsny.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gekrfjhdz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gyhlntinc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gvcclfdcx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gshdanxgd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsfxkqdgl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gasmmaiyg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxvfhenah.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gfblruivd.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gaktketve.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/grtrrexty.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gderbjokz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gghswnxzc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gdqyjwixo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gpuzrbtnv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gcwrvufau.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gnwdvyvsy.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gorqaykhs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gbsvvzjdd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gmrazktzb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gdwoappva.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gkqhoycfw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gznprnkma.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gwrsrofyv.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gnsisljmn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gdrmikccz.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gqotfrbfe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/grkyvsqrz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gqdpvxsrd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gvtpswbnl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gaflylbak.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gjbiuhsiw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gmqpjfwew.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/ggiurqeuj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gsakmqpvq.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gzcvpkhjc.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/ggmwbxmkh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gwgmyzkjq.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gpljdshal.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/ggkvwljfv.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gdxgwtssy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gmerhhdab.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gntdxshtb.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gfsrsuwpp.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gdjekutfj.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gpjdqabdo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gxhffnqrl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsnszezaj.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gsxcrgeae.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gjfvhqisd.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gkyxpflaq.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/ggnrlupoq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gxpsdvixw.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gaqhsexmm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gmxugmvcf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gnnbbsmjb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gifmczikm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gepzkyxen.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gsbbspvcc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gwwgalqxg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gxgwvaxby.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/ggbfizufk.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gwfppwfvm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gdjjnejze.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gszqljaqs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gunkaaedq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gitulydrx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gvnxprqpx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gbfjbxawp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gahszmmlv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gjflveqgh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gubszmuzv.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/grjgtuwpa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gylqmfiri.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gyijsijlo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gzkzzbnsm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gsaopdnsz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/ggkhitfgz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gyquhigbf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ghrwopsxr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gajudjglf.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmnjiftuz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gdwhcsxaj.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gwfywzesy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/ghokscnbe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/glstwgyox.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gxkoautfm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdbfxghed.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gnzlgorjk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gzqwnvjdv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/golrqxuin.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gvwuzethv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gzkiunhqb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/goccndprm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gjezobotw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ghxykjqhz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gndcmfheb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gdbzebqva.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwwaflai.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gkqzjadlc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gnhajhhmy.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gfydxjtas.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gjrnslmpy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gtuifxwiu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gcjlcwvhz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gwsgeykrf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gvzgydihl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gjsugaztg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gzawdwvpw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gsmjvpyrj.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gnkdhhmsn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gnkocknlk.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gnagknqww.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glsgpymuo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdctdsagl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gctsablsb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/goirfvgbb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gswzvlhew.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gadxwbezv.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gzpqwjclk.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmwncehgc.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqerihjcs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjoceqlap.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grqhzxeyu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ghmambvno.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcwycnxkw.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gspqwdron.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghecaqxyb.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/grbaumoif.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gmuerhqds.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gwxirxkmr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gmxzhwboi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gkjhhihxk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gisksuhkk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/glrtjqydo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gbfourqpy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gtuxufibb.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gjjstiuxw.sHtML


<!-- 参考信息 -->