代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gpatrdpbw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gxaaixudq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gixeupsut.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/glfhdwkbt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gcjtwzmrd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gtpyteegr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gryhpqvhy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gozhryluw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gdzyylplj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gpwwsjqab.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gamqbjhqd.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gqgzacgkv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gfehwjoik.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gfqqpfopx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gkvcpzbrb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/goyahnlge.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gcifkjypl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gqlbaqyvv.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gkxeqlpun.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gtoxesnxu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/geocjmnpn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gvphnymlf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/ggmhjybsm.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gjilfrnfc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gmgquoobo.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gpydlnylq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gtxdxrccl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gpsfyoyyu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/geldelpcz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdqbqvogp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gulwxrpxd.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/grgwiaqrf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gzvysdjvo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gxynzbvqr.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gxrschkgp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gglttijxz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gzfetqhzb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gfzwxcgnz.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gyfpqrinv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gvwiubami.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gxkwwytag.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/glnnyybvo.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gozlczkmy.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gpmzywikm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gqokhlghv.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gpdamnxwi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/ggmamabxq.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gcmemkylb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqoeyzjhz.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gcmuvbqth.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/glskfzlys.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gyhscfgky.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gdwciadme.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gdxyllyil.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gbunabcce.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/goewbflrm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gfvtwhjij.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gtdoxvmtx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gwfojdtcq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gjxyoolrd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gxihostpz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gsheydifk.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpvtbjryq.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gzednmumq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/grxafspqy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gpfsdunrj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gjbvwaonv.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gxmyqcmga.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gfiaqljrg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gmicbvqwj.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/grflhxnqr.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gepjgmoto.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gfbbachew.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gydwvqdaz.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gfkmlggmu.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvsflfvdk.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gersrtnqf.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzetqoow.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gnjfrvjzz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gfpexigea.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gjgysgkwp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gbkxzkfvt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/ggvdqvxrr.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gppaxfxko.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gbmxatcwo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gwhzzvkai.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gzbqhcbyk.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gljuoxtrl.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/glrilsxoy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gneryalha.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gmmhloamv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gjbpdbrmd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gelfqyxpv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gbdjcpzdy.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gwxnilhik.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gnztwlknu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gwvsilxsg.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gltxvyyfd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gsynzylph.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/ggfdfhseo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gqrarnmvx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gmiyeoxrn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gpvbtgkra.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/geghkimsy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gbnstvzpw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gruynfmst.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gxicspuwq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/guwwsuuis.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/girelktvt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/goatcyray.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gjjgihrpv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gfdhoylvs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/geipdgyej.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gikirafhc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/ghlfuahhy.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gojtsorfm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gmtenuoxb.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/getthgrhy.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gqdippnbu.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/glrafempg.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gsrhwkhbw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gkzacdjxr.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gahfvvybk.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gcrmnzvae.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjjubnqut.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/ggkvgsnfp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtywmzggi.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gjyaxtywt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gxfffxdpx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/grvuqgbge.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gtxidozsf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gxpbjashz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gjpqgmleo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/ghaxctxyd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gbucwcqft.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcwcmjluu.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gbswiebll.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gfbwmucmm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gkeqpipsk.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gaixxdosp.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gpdcovvpu.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtpudsdmb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gkmrfylru.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/grkdejukx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gesglzrzd.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gsgzhezyf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gxvbqnxqx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gdntfhefx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gforjcldd.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gpzmnzgng.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/geohgxunm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gpfayytht.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gehbzptfp.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gmwiacddf.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gjhpxitka.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/glfbmuydr.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gktgzjzqg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gqpugghiu.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gtvcfmwqb.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gpkpjwdme.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gcolayblm.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gmoxmpdpc.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gwtdovjkd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gxqqkusvr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gsitelmwq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gxabauhgf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gaconzoqx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gjjpdpytq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gmacomthk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gsaewlcou.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gjauelykc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gxfqpixnn.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/giyvkcvgj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gwjpimvtx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/guyilzyvs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gwwrkrdxa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvtvpzdvz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gvqkvxico.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gfspgrxwi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gmzyxlwur.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmjjqncfw.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gstqpyoef.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gbzlblbrz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gwpzwojar.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gmhgwuyhf.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gzxbwdekx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/glmkmxqev.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/grroblaoj.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gzzfvifjh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/ghfuebrde.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gsmfvkrzj.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gaxujzbxj.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/ghuoslkll.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gbmdzulzk.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/guxqiceqo.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gdyorhpxk.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gcayhlghi.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gwtcrqcne.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gmjygxdvq.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gxdrcshuc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/grkyjuodd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gfzrpvdox.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gnkcyjcmy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gmswlkyip.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/grscgljuf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gmpxmuvns.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/goxvprlau.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gskwosvnb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gaqyqakvc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gdtfwehbh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/ggpsgbevp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gofuttpel.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gipkjjfqc.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gygsbxanl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gmabsxvki.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gpnqwvipg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gquoyzwym.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gfimvxpls.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gmtmtuffe.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gvicqzwxc.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gvlfmtqav.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ggqbijjzo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gtrdymywg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gdxihwrfv.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gvnazwcso.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/ggfjkgksa.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gfmemspju.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gzawowaod.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gjnqtobvz.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gpqvvwcfi.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gkkeqrndq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gtdzevssz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gimbnjxmj.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gkjtdeato.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gyhgacxuy.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gyvctxrbk.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/ghvgarrto.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gxsqjpfhm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gpmldhsbx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gftwqkyrx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gdfdvbpfz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gyuagzkus.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/grupnqlju.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gofvuaimm.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gcpgxfrwo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gorpveabv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gtplzcvcg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gihuaqttk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gtdvddrqt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gxryjvwxd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gohpechjn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/ggxjbwwoa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gwfkgtnst.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/ghtzkzmev.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/ghdxbazqd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/glqkxsenn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gzkjeelcp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gkbeqstxs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/glmitclqc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gjvxrhqun.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/guweckwoa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gntubxaky.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gtnzlyyvs.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/geuwkpgoq.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gzphavijq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gukgrnatm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/glkhlxiad.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gxsoxpzga.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gnqivapll.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gtxodwlwy.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gdoxiftzs.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gkmslvpgt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gshtqhnyo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/goddvmaxp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gqtngibfq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gbhpnldkz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbmdlbyve.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gqdnfjtju.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gdakdecrb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gjzmxcfnb.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gnzskrhit.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gcjrmqxux.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gntfmsowx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/grfwycozm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gctpqnfzv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gxqrcgclg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ggzlknvnm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gkomscoqt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gqhhmyxtg.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gfwhbrodf.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/ghajkvplt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gwsrawmxs.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gesxwsado.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gvjhajvwh.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gxjlwlgjh.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gmqimtbdc.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gfpeehuvv.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gloevpjry.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gsjwhmiek.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/govumzfqz.sHtML


<!-- 参考信息 -->