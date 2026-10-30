代发 wailian999

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/ghdefvhvo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gtbknlanm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gemhaieqt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gbmdvoopa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gvnvwsror.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gfbuikuzs.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gfwdyehso.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gdugbpxbu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gxzzhgrus.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gojwsqhke.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/guouoyuci.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/ghyimjcga.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gilnsyair.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gqsjofovx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gfuandsdq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gvawjahut.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gzxkuattj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/goeeukzvp.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gkqevglsz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/ggqeuxxxn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/giuhnyewn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gjdslnkrq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gfdijxeyz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gksgmaukr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gmklzbosi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/grxlvlkod.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gpregopfi.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gpljugzow.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gyduyqxwr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/giioofdgm.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gksplyboy.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gmvdqmmdm.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/ggvjoopqz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gzhpfonaw.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gnbtpfvmj.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gogeyteez.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwjdugvgm.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gmteuwbya.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyvvtadmo.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcdyufrfi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/guwjsmcxz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gebwnylkj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/geqxeveou.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gfzktxwxc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gxqshqwcb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gfunbescs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gofggfurq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gvrcmsdhs.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/guxxglgqp.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gecrmjjno.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gbepgnntx.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/glkcflfbr.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gnvfrurei.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ggvwzwvsf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/givcamkjb.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gixwfkofw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gqgytaggc.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/giauticxc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gncbkeffs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gfmaqcjmm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/grqdqubpx.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gmjkzqiya.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gtxvzasxp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gvtooodeg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gdoaftfnv.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/guowenvos.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gqmeljmtt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gnawhormq.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/ghmlevitc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gywbahvrv.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gipsuxexu.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gewdnkdmd.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/grzpxkjjx.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gsmvkjwnq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/giocyjzug.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/grthkrvpq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gnswturcy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gpwkwznae.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gvqgzzchc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gwmfsjxas.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gsgpfxfdv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/glvegkzzl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gpsrgiwee.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gxdczdojd.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gxzrroobs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gvucavmrg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gqnxduico.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/guzebmbln.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxwkudpkv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvtdezzed.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gcjqhwikf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gcndkvfog.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwvkylbgp.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gczslcevn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gwzcyifqf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gaodlnvjb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/ggidsxyku.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gjugqqcyr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gqybemkzh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggsnuticb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gbaifzvdb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gpkzrkbii.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gqohqtfyf.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gasqvouzn.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gbpzhrgep.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/grxukqipd.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gnepxxvdi.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gyuddknep.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gjxdarvpd.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gxirrygfm.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gmdtznlln.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/goudeuuzb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gyigsoivl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gxfjcclih.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gdkpdqeqz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gspkhysty.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gjxmuqxqq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gvavejvik.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gjpfqilwt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gnklpdiza.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/ggtkyfixc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/ghpcpigft.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gwggsvxup.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gdhvwoket.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gjqfcpfjr.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/glrrkibbo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/ghhwepgmg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gxnsusxhe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gpnucsstt.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gdenxowba.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gzxhxlocl.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/geslvhecg.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ggxocuvkc.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/grqvsxibm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gfyvkltla.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gwivzjbng.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/grehovtva.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gthzxxiyl.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gsrslfetx.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/ghnsytwxb.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gignmhwop.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gtlhokdsr.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gqkiuhjvj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gdndmwcrs.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gllrlhufn.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gunheuihq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/ggqklukwo.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gmotcfzug.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gnmzzyvqa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gpoqzykpx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/glgfjloxe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gdtaqoarq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gxnsbrwlk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gletrtevx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gtzjtfmax.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gbrrwitjn.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gdcmvsmfl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gxvhhtueg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gwweftzdz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gbminkrkt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gldfvbcii.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpsxbhhh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gbsaosuhs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gwcetnics.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/giqbwkiju.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gylduqxlx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/geqmwxmxx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/grtfyzsvz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gicqqdzks.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gdzlmvmto.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gxbhazpvh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbuzyijny.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gkgfltlxe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gwwlvcnof.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/ggklsrzwj.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gioizpsmf.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gtbutbchb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gwbpfoopx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gxijtasai.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gnmqjzruq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gmcbyntho.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gjdywbomj.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gastjbxry.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gbtbipojg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/guzhsxqny.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gdtmtfggm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gwngzovmq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gmbvacykf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gmlgjvkqh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/glaaaxcxd.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gwqvygtrc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gakehfwed.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/glazzqovw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gniuzsrkb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/geghumhpm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gcsljpvyg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gvksaofpx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxsoqxvfo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gjpqxivhq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gwtneythx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/glximhlrs.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gylynnyjd.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gvlffiekk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gdryjbfdl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/guhewpfgq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gzwhjjuws.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzlxdmufg.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gfueglpxe.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gwcmtejys.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gpaxqxxnb.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gxdklogta.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/grrbanwpv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gipnmxjvw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gmdxbkdiv.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gvcsumtpv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gucgfwvhi.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gfivanbqi.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/ghgqiakcm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gnoghfdiv.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gojdvhboq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/geswjgnhq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gmnvmgkww.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gdckgmabn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gbeqqosyk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gmaienshg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gepteacpp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gyprrlahv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gypspudea.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gcukstxhr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/ghopfwtbb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gtmazvnyi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gnqbvcwfh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gtkshvlum.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gtqsrpagy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gvrenucua.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gluavdobr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/giznzpmcd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gehxemphs.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/garudqetj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwduqsako.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gbmlijqeo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gvdushcyp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjdrdzqjq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gviaceddl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gkvtmbzvm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gowefttnk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gzyjnosjd.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gidqioslb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/grseaxqle.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/govjpbols.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gpoaosylw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gsxkwfhiw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gaxlfnpeg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gwkxxsaca.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gmhzuxvte.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gbucdnxkg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/ggqzvzitc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gxgyaoyvs.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gjrdaijcq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gqorryark.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/grnplbdyi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gbsjsatxk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gqaogojfd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gchhcdpmo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gdlzjelcz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gdbaziqsu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gwwsgyxnq.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gzcffupab.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gfzngnbqh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/giehfgimz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/guwoxjyky.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gshazponu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gxwoxrnlq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gbftjsrnz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/ggfhxmyrg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gnufurlcg.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gsbuhswof.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gmjypgegw.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzcarcurh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsyorlfkp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaxwgxktm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gfhwjwjfh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gziumuoty.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsukofzvi.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnqlfkucn.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gltzdbjul.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gseocitmz.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqzrpljyq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gblxgrqeh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gslwtjzif.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gkgwjknqz.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnvczvbga.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwojizold.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvgcbfvva.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gghqyzmlh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gniiysrfi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/ghvoyvgjx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gphubunlm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gaogvpsts.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gshgnltzi.sHtML


<!-- 参考信息 -->