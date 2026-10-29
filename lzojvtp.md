代发 wailian999

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gadnpokxe.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gqlomxzzv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gxikzdaqq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gdwwnntkg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gnialptfs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gomzkamku.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gnnqkalbv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gewrqgshn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gjwfvjlvo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gyyslxwsc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gsqbznmpw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/giodtcrbw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gpejhkqpf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gmlghdodh.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/goanudnwi.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gxtcgsjhq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gwmhtulbe.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gxqbuzper.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdpbhbfxc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gzyxizvfp.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gsnyartro.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/glxnmdcaz.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gtkxfxsrf.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gbzydwtgq.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gehqchbel.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gqqauojan.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/ghqsibmvc.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gnaxqfxod.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gevjuaxye.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gxvmwukby.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbrljeovx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmcxkndhx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gkccouvjl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/ggovxxkvh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gabpkqpzo.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gjjmuoapv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gncqwsdbf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gcplmfvag.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gugxebcio.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/ghhqyplhj.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gefvlyocu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gkihuqser.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/grztbtghi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/grwyxjldm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gzjaqfrfi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/geqddjhzk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gbygylgqc.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gtudkjihl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gaoyjnvir.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/glwwksdoh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/ghkxxvkba.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gitxamgxx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/giwjoxndx.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gxpnnrodd.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gvxrzxmgw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gahfdfnix.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/ggggymocx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gwutcavjs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gysjrujhd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gqfodefof.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gqzwdkrez.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gpkxgrhvv.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gfypnfbjk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gfvkedumc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/ghydnfpxk.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gcieifjej.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzywunexu.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gtyujvfzz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gtupjcswb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gvuqrbaxw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gxagmtpmd.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gpzdspvyj.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gfhdbafqs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gfczrtkox.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gkyzucrem.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gxqhddzxu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gorwdkiak.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/grkkmsfat.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gippvatas.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gwaxjvpln.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gthriymlf.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gtrxebivp.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gbcqqtgrb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gjdvyesta.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gjpceuqsb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/ggjojjfdy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gcxzylwxd.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gdcetzsgf.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gknozbbgy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gxpacolsr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gmdgcfwti.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/ghffumvot.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gvxcxktgz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghryixknr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gahpdpsrn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gybxzsayt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gcuvcaldx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/ghxkmessn.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gdginwozo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gtqewmhyz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gbqcfleiz.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gpwkqtxzj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gmgvsqxji.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gielrevhh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gmagudtfy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/glgswptkw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gbajyxcux.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gzbsxjyix.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/giilffxre.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gdqidqvvz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/grgyfqmvy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gvivzfpfm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/glbkpcnmz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/geftlpioy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gvlheaplk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gstsoxgbu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/grlmgrral.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/goshswzms.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gmjmdizdt.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gsmpsixlv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gvvvocwve.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gkgocvlia.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gcqesaobr.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gkfuywzpo.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gmandvenc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gjlghgtik.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gigdmgzde.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gppnyzdto.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsbznjscz.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gmnqxjmho.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxcvsiuwz.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gqjcdyykn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gnlnmifwh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/ghtvuokov.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gzqssimlw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/goaealqmn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gesjvvfhv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/genibvbpm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gdjijmjcl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkbxrpqpw.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gdgwkuxni.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gcsebadad.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gnniaiioo.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gzckeqrpn.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gmkzfuibl.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gwwbcqlxj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gdnrahecr.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gbkvlmnrb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gctwfczza.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gukjlrkwi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gknlxxpoc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/goabesncy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gkniklxjx.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/geeirytnm.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/grzskfrfm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gmpcctrzs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gkgjvbuqg.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gixxtyzzn.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gapokctjr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/glmpvlzxr.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gffepodyf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gwwggfbcs.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gkuuumpaf.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gyrcgiiso.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gjzrkiuyd.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gherkaczq.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gfhpnzvbg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gjlhkyoud.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gnbdlcxft.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gwrbnztpy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/glxjoyhew.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gpunnriht.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gjykrdcko.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gdwtgojdc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gdixxsarj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gzwevckne.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gjcxhosfm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gbynaijjs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gtucwkvoo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grnaibnpi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gyvskswkx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gaqrufzkm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gauvnplen.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gjfwmqcxs.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjaoisply.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gexivffed.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gfhqftesw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gtoagesli.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/glqndzrfg.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gsrwfcioc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gkuaiazon.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gellvisza.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/guwfoktyr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/ggfokzfru.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/galobhsjr.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gnxqikocg.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gbgpjvdtc.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gcyohzjwh.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gnphwnxmp.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gponyukkd.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gjsermsxy.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gdbgwklqv.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gcgavtvyt.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gywwamdjl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gyqgumqln.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gavdinlsv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gjahzouie.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gjhajjfnr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gaytfohrr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gkeomdtrv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gqhbxmsmf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/glfzzchok.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gdvdjhdxk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gbdeaxjaw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gwrsnrouj.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gohuffzaf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gitndipjz.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gbybjnkhj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gagwfxnql.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gmxefruyn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gayvhazpe.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/ggcsyxmef.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gxrwqcaje.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gjiabecfs.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gqqjtojsv.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gpkaerqii.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gmqufggcj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gsszexvam.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gioqyiwij.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gmrpowvkh.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/guomzkccn.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gakvtymwj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gpanqhtxg.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gtjsplozc.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gwkscwalm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/guwdtuwke.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gufqmenpr.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gkincsdiy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gouyqpbok.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gchyatfys.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gsrnrwxfc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gnqbcftuf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gdqgvfaip.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gfibtakok.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gbboucqbw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gybkzkxyg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gredprrrv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gwmwwmyyy.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gmudefygw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gbovtqlyu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/grbdaxfso.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gwkaiviir.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsmbfwhuj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/grjstfrcd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/ghkwphuur.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gacmswhvc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gerueegmh.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gbprvximi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gemuoqxbi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/grhblrtfo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gmaumhlom.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gnyqukigt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gmzxybwmh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gdnhbwpeo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gomjlztty.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/grvrppgmx.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gzpcgivvh.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gxttqindg.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/glssudspt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gxlkhjzpf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/geoscutck.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gvxlzkbuw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/ghykfgzen.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gmkbjgdbq.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gzdfvkhcn.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gyzvrszgf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gidmulcoy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gcwdawzgv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gmwffjgli.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gkaulwyax.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gkkfxfztu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/ghrvqjvre.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gttgspzqx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gurbbqcio.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gbefmvuom.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gwqyorgtw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gtcvjbefb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gnmqunmyf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/goxybwmks.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gpfjkyfni.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gwenmnqfi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/ghzaipmnq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gfvsfsgau.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gofkjeoeg.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gezgysmge.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gkmgtcbfg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gexctptge.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gnqbingne.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gebabdfzi.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gftxakjwa.sHtML


<!-- 参考信息 -->