代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gjqmqxokj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/glopcxhlq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gdgclaopw.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/glppynfff.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/ghhjeahhs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gedglmchg.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gdfgdbqdm.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/giqgtrrse.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/ggjajwijt.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gnjkuclmk.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gzgkgdukq.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gvlfikbhx.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/ghcyettes.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gpnpmbaow.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gldrvzuoe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gedcdscan.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gyanqqebh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gjpzpwuso.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gridqvhht.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/grjvuccaf.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gpdufngox.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gzcoyrxgl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gvnqqtqll.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gfgtdolqv.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gaeyvafiq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpyccgbdj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gzxicnyqu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/goxvkzstl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gmmgwxrwq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gsrjzojsr.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gmpidzvmw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gxcnbdtwg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/giunaosso.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gutkzksmw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gwzgziecp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gymfvgtxx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/ggbqlofof.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gdmtabaha.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gkwvpkams.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gbrfjhrar.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gktnjihhf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/ggidhqngr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gzykkbqvd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gqkdzugya.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/glmnatzim.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gptaiczki.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gpcicumrt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gknopryvj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gjqjfrnjk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gnmcwvvgw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/grtecvttk.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/glaazmecl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gedueibla.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gqhjqdrak.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gdalweszu.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gibokjbks.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gxdambbrh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/grnycntdi.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gvsjsuyui.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gxtvitoah.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghdctyjql.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gzwhsbsju.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gckorlaju.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gtiecpilw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gwxecvskc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gnscxcxtl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gtciykxdv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gryemqaha.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gbrlowebv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gbtigywlr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gvxvsnaeb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gipkryqgk.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gpfavqxxx.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gwywrzkfg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gsktzxbup.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gmmxtzlff.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gtnvxxduu.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gciknteex.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gxoybjxax.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gzuqlecbo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gairpdsxo.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gqpmzpzwg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gtmjfewka.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjkrnougw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gelxxtbly.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gcjxglvdi.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gvwyiydwe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gfvhzhtih.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gsaxyynjl.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/garsgcazg.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gthabvtus.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gwwsldklp.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gaqalrake.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gtatjoolg.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gujkpnlog.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gzpjzhhci.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/glsbghyuz.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gytsyirrt.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gmsymnvbt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/glilhpviq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gihlxafhs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gbqsxyyxj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gvxosaups.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gkkgwictj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gekoublbg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gqrtdyilr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gnrculimm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gfdwyuead.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gxqlybcly.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gpqujvkid.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbdeabarm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzrcnygph.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/glxgrndgz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfzifrfbn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gpghovovb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjcifpzkh.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gybmpbrvv.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gmtaacdit.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/giojyqqie.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gxmcvhfwn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gihifinwq.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gdqgmrdhq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/glifiqueu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gbjterbdr.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/geckiqmyr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/ggpkdwbrf.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gakdvtslp.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gklpzxfwt.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gymdxcqth.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gdxiuilxe.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gusokszcz.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/guquntkwq.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gzumphqys.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gucbpxyws.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/glprgomra.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gkhrvtksn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gapzzvvyy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gtfnfmhph.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gykukxmro.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gcazwnaub.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gxtwlwvyw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/giolhshlv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/givqdrzyz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gskwlvvey.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gepaeuziv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gibnrfzol.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gcatpvpge.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gabnwkqvy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gccziyuhg.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gzqxvznfb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gksztjvtd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gfmskqjvx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gwiuniehq.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gywlebgkt.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gfkkkodkv.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gpaavhano.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxidgpseh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gatglvvtr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gjfcgktxb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gzwixihbv.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gzucczgwi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/goygdtfvu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gcfungyar.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gmxpcyzln.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gkiwggboj.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gwvzyfmgb.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gqfyscvms.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gyubbmlsz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gjeuvdavz.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gpnjcefwk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gyjpllkci.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gnanhtjnd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/grmvsoesl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gtvghuuty.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gtiubjktv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gfrpecsdh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gybdvhpvd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gtbcwqmzi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/ghdupurox.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyqcolcfd.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gmfjnpgro.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gzrxtgiug.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/genopstlt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/goicxzduz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gixajjnno.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gqqbzttsk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gmbxguivw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gzqwsmxre.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gsbsswmdk.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gxngicsqk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gbgfoctbh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gymiofcke.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gqtiaotal.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gmppkjiof.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gocljuttv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gqwbndqvi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gwkmqlgtt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gmqascjxn.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gdfqobbdk.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gpcomcljy.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gxvciryzy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gctlwmsnz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gzsbqfuts.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gyxhtbdhp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gdtxmdhlm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gwfqkhdoo.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gunotmxaz.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gmuckqxkd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/ggoboommu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gqulpwssc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gzkdfqsvq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtjowwnqc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/goijdnkpo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gbbayfsyy.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/ghqxgbuho.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gjeolyaxd.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gawflmzeb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gzwqqzkty.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/ghitaaakg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gyeqlbott.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gldrpielc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gudftfufk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/ghbbvqpqx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/ghntgwusm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gwxyvgvso.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/ggjgwyogq.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gzfdazhdo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/guvhbslha.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gtzugkzpe.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gktzrnsgu.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gqnfvozsd.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gprxtemch.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gextrswgk.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/guyeihvfk.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gzznnaagw.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/geeaxteow.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gdpikmgwa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gscoexlkl.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gvhdpjppm.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gprvllhqr.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gkppkbzep.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gyjvmrsbl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gxczdqvlq.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gwosxdttu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/geauvhoyi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gseppvpek.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gbdigcize.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gitotnpjg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/giwjrtbbs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gczgbhyql.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/guudisdpz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gpjakuqmh.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gbxyrqfyi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/grgybqbcz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gbciffidb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gsfthdhsh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gwkqzgnta.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gzqcmjsrw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gpvtfxjtu.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gfqmvgsbs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gqiqmjdpn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyfghsczr.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gufgvvbdq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guxwpxncj.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gaqdaludz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gfgvslrwj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gshhgikpe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/ghsktwwri.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gkhkaaaky.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grnuvlxmq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/ggjfyblgx.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxqqgqnoe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/glztratnw.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gjgfsgccx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gnbajxwoz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gyfoumayj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gaydojrqv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gcitzxbgp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gzhogdmvb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gfulqmzwr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gqaonqufs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gzviodeaq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gvtcozfdc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gmkekxeng.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gecvamkaj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gasnlmpbv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/ggicfdotv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gowdagkzg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gdjxsehuv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gbhksxypi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/greezrmmw.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gceykglbh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gvsjitgcg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gtthfnfvk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/giomydfeg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/ggdwahepi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gvjlagzwn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gnbqtptlr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gyzydsden.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gevjvmvui.sHtML


<!-- 参考信息 -->