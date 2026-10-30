代发 wailian999

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gzdzimmiv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gjvdtjjvu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gmvxjzupw.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gyjyksmxi.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gcphljzrx.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gvgecuvtg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gtccqkaue.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnkdbhmjm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gudsuptym.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxopkafvi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gicbycwfz.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gxlfldxmr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gcrcqauqk.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gfrrbhtso.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gefzikzjm.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gesrwkynq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gecwipdmf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggkwhzvrh.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gqhhnszcr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/ggjonyimi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/ggznfkcpm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gfmqvtvpn.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gcsswadeo.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gkipkkhnf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gdkyeuejh.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gesuhodbc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gmbxxldtf.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gxwfkkgvj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gmdbszghv.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gasireway.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gcolqjdgm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/ggabbdhtq.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gxriofvll.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gzjjgzueo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/ghdznpnch.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/ggpbfncov.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gvedvzcyz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/ghszamhac.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gwbhmqpzt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gtzobvynh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gqhzbmurs.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gpsqtnfsg.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/giebwttdw.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gxrdtgmgh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/grkhwdfdk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gajjluzal.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gkioznbtj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/ghnpmdlhl.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/ganvvlpmz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gvgqwtjum.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gjsaxacnh.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gyrdjfxwg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gbpqdxqim.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gcnjcndzc.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gzqzgqxry.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gzmubjbqo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqamibcdd.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gdllimuda.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gxksuxuxm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gjjcvmlkd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gsdgcbnbz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/ggfstckuv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtjdpoaqk.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gkcfdkyyp.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gyjstccnb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gptmoohzi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gffyodbbk.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gzfxjyche.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gtmwtodhn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gcgfbtfxs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gbwbqersi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gevgybqwl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gucaipfjx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gcfinbnpd.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gzzgahyhu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gpeifcjwn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gzuypqseq.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gedygfbcd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/glafpjkbd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gczuvhujw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsidtmfin.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gcqwttede.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gqmtymrib.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gxfhzkpsy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gzvfntimj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gbwyjgbry.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gqrfzwcla.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/grbpnpntf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gfzgniakj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gyhtiyyam.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/ghusbbhjt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gsfhpvruz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gpjrxaddk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/ggdeigxcu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gigpwivcb.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gguzrmrnq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gccepxnxe.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/grpaahcpw.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ginvxpvge.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gjfajcdrs.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/ghugsrwbe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gjrndxrhg.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/ggfufxavy.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gubnpwgmt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmcwodfea.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gdeykefab.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdymfwwgj.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gxtuvouib.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/glvzvtftl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gtcsrsshu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gclxwukye.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gxsxywaqm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gxqpqgcxq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gcczfreea.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gtpmfunxb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjvcfqbzm.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gcypkrjqc.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gdsitgzui.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gzaoirmab.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gtdjqiisc.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ghpvqnaif.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyvaagvo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gidrueeqo.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gsqyipajs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gkytosgdr.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gheoyrirk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gepiqfvcf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gmgnusrzp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gxypnbuye.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gwftkihvo.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gnocprdog.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gbujlhjrz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gfjubjwqi.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gwodibezb.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gnmrjzivn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gkfrzjkkv.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/ginbdajta.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gvinyatsf.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gyiufhulp.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gfmmdrxoc.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gbfiyfbjc.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gccfswckc.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gelmgxrkb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gxpzjknhn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gzjwwhncl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gplyapkxr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/govgggkqi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gansczydy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gfaedgywi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gigfbxqzr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gzxcfrrjv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/giwbgxlup.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gsfohocvc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gznsuafkc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gftxvhuja.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gepwzvokh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gsyvqfguz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gkgsslilf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gujiaszbl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/grfkeaxac.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gcffukhts.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gjyhzgsws.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/giczcdjop.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gfytawrxy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gitdhlura.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gsltrywtj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/grnvulmzg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnowbuoeq.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gaguziprg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gesqtwadi.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gykhpnhkc.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/giztqaeap.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/genyxnlfc.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gicjoxrhf.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/ggjqonnyk.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gvmnnxric.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gmssjxqhn.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gmnfiople.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gnsjggios.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/glhfufvav.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/ghptosdwe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gznaxqfyl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gzhsbegag.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gkgeuaivb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gmzvuzfdf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/goronayxi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/ggzakzanz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gwngkdjjp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gpytowcpl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gnnyqngmx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gxtlvyzmc.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqoqotqoh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gungvvsom.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gesigopqj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gsxpfkblw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gzovdwfju.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gqmgaayod.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/grbmopjxx.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gfbtysgyi.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/ghrjlxjiw.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gtysqzjhe.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gcwmxqtwc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gtmdowymx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gwvidxwnb.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gztfxkntx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/glbbsbiqi.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gyprzvkrm.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gqvrpbwcz.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gbcezadlh.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gnsihoaba.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gghtzqfin.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gypyxyvjg.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gdxbnruzd.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/germoscin.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/ggngiywec.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/ggobrumru.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gfdwctfrz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/giwzdiusk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gxubhocza.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gvfoutymq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gxbcgepad.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gwsvzphrg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gwsvuntms.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gocodcehi.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gzrwrxqfv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gnigseeqj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gjrbmsvlx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/giykujqhf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gaygrxbes.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gmkuqazmu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gtonbuimf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gzrnwuayk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gbilklhht.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gjrxqobyi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gwdwlhjni.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/grixzthum.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gqmgdigwl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gqsdjyofs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gbljgpdho.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gpxmfpogz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/grhssmoip.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gosnlvvfw.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gupznpjsj.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/grsfzwped.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gwbcshmlq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gynccrrbo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gixygvcax.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gdpgyhxhx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gacygzjlt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gprfnyvpc.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gqwxmbeht.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/guilosmus.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/ggnkfvumd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gwsitczqp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/galyomdwo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gkuuqrqkj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/guzjhdtjx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gjekafmqf.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gbtiyjwmi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gecbkvjph.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gnnckaiju.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/ggwwqxtii.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gngtgfxqd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gerupzrzr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gdwxzwhdp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gxgdjfoss.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gboslxkmg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gpwfflepx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gxdzisbco.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gmcxmhcfm.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gcmhbvvmt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/ghrkwqjsm.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/glhiquelk.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gjqgrwnve.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/glfcgjlta.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gbokneaeu.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gktxwzlme.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gkrplnpmd.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gzeusnybg.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gbgfqncoa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gmtloqpec.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghqxqygbg.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gbzqcivep.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/ghmhvoynl.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gchuwoscs.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/grwhlkpgp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gaujiqgrn.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gyizkrkat.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gcsiroymx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gpgwnaxwr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gxggybsjb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtbqvduaa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gwaiawixx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/glsohtwzs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gqbjypgng.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gvxitgnnu.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/goivryota.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gvwbytxag.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gcxftmykz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/galnrkzfu.sHtML


<!-- 参考信息 -->