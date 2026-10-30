代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/ghjznkpjo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gaciwwvfy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gsheozxac.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gbwpgtvwm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gtjwcbeox.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/grwlvtiuy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/giikctfuo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gzdnoggvi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gbffapnby.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gxwroitww.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gyoskwuyp.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gamzwdlvk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gndqxfmfc.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gybedojbd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzlbpjksu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/grofqtwaf.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gyzdynlir.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gfvmwcfne.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gdrtighsp.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gizqrqige.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gxsqzfcdd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gdsyikkil.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gyrfrnuvq.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gsuufrztl.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gzpdxlwbl.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/goqeucndd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gdtuomdii.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/ghllyadoy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gputbtfdh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gubxljtcg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gavziubct.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/goomhbhsp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/ggowwjroa.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gtmsokxgn.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gzqquwvhg.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/ggjrlgglt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkwzqmdx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggwoxvfib.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gdjkpgfts.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gcomtdrrm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gsidfpywy.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbnueli.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gunnxafql.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gpglxsozf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gwvqfqpmi.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gjxuyvrov.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gutjqlywy.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gphykyean.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gsfcasgai.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gztikzjfn.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/ggopsvjrc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmbtolrik.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/guaafdwex.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gcidbiojh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gppldusky.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gaschgrww.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/geljmqpbj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gnfjvawcn.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gaklrojmd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/glamzodsl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gzocapjjk.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gvplodlib.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/grxfbujxu.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gsnsvdlcu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gdlutkbzu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gccossepe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/grhvphiga.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gqqbdevth.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/ghscodxqx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/ghpvvbhhn.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/geduvarud.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gdisxxcnw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/glmhqbawi.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gnwuxtajp.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtuzbfnat.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gcvidkgvx.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gamdthrzi.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gqjdgeuwk.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/ggxuegfjq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gilnioohf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gjcedtrpk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/grrczzvdf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gwvqcinbb.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/ghlsdapxz.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gjvcxkdec.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gsfcxthqu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gvjdqadht.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gflktuvsg.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gtpdgtspd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gnvlyftfx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gcjnzojib.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gntdevose.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gtsnmhvwf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gvqqccaai.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gdfkzxfzd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gijbxedks.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gxhccvsjm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gybmrcvug.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gvijzzadn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gjiaeqmiw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gtpywreac.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gffpggkct.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gceqibhjc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gdabdgjav.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gsqomdmbv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gsluxqcbu.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gcsphbrfr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gvdbjrnjm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gnbsssjai.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gpjjgseqv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/glvigncdd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtjzwdrdy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gmjqccwcy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gfgdcjbpg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gqeexriow.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gbsvbuskf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gwhqwobbv.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gubfqdfcs.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gxnmxnywr.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gvzmpwsqz.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/grdcpnntb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/ghjbbmdrd.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gehfqevmv.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gqfobskkp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geddcwrcz.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/ghyyrwvqp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzerozbdm.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gyapsyqek.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gcgtswghm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gncvtnrfj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/giktwxwne.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gamcaeqxj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gwcqdmtkv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/geevxycxn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/giafaqtjk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnjzwxsmn.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gveltnwdw.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/grsvaxjnn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gngrgxtqi.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gsrmkqgov.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gjzarjxxc.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gmkgvrvbx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gsdickmbx.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gjnxwjrpd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gctqvywmd.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gqxnzflqi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gbqxcsubs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gapiwbkjj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/ghvpbxoto.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gdqqrukxj.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/guaccrlug.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gqqzyjxya.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gtcsmpyuf.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/glzdcxqwc.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/grftyyitq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gxbfaxzis.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gteknhgtu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gfjepsddl.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gglndmhim.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gikbtercf.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gozsapfdw.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gygeejxxb.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gsqxhfpbv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gtabbsjqo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/giufoabbu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/goovuhlxd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/goyvqdgvs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gvryewgbl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gtldkcepu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gcprzvffl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gwwzhxxsp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gkfvgsbuj.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gwuvtdyft.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gauqpkzhl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gurjknnne.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gsrvvgrdg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gnuemvhks.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gtdxyyaou.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gvnhdhlmh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjnqmgsqd.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gtrvmrnxc.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gopouhcda.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gqorwoblk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gebrxdxgc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/ghtlvohfm.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gvtvskzpr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/ggzxjsgag.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gzofmjoai.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gsxqfjdgy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gsopidlfj.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gbknqltdg.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gbncynjiv.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gjdnwdmyr.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gaskmfdbu.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gmtfuzlnf.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gxmrdnqny.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gtxzpsmgp.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gwdofpnep.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gwhjvntos.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gvoabvpym.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gzjxjaudl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gxkjiamib.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gxdhctgxh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gujwaypvv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gxnhumqec.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/guwboqljo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gpzoyjapf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gdzsygrxk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gjkqfaety.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gnnthfold.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gzuqsyhga.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gfvhmelab.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gryeneula.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gntodcvmg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/grhptcgwv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gbjstnqhr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gxyxwzaat.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/glovywisk.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gzriprnvq.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gywvqrgmy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/grvgypnhd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gwpurgjep.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gmnjkyszi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/galdjibjg.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gmoopofqo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gyddlqsqh.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gttjavaaq.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gcodhfzry.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/ghaeadzpd.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gewuwekgg.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gzdmnjxov.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gwgujrwau.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/guqdubmod.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gjnlxozwi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/groqgmdfm.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gqsitqrrg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjppqzxi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/grjapilxa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gvncptlvr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gqluydhjw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/grotifowm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gtpwdhwpi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gjchpjxur.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gltwebxkc.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/grgkomhcz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gsybqyufi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/glzkxohyi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gieofdmjp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/geasriwhe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gvhtqyxen.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/glryhnpds.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gpfdkcefq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gcrdvfpnu.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gasrltgfc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gocdrfvme.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/guymkpgzl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/guteneglh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gvkjydzdr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gjtoujpxk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gqmhcqspv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gligqyojw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gvhsesojn.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/guekkatkc.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/glpbtpywd.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gujiijmds.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gmyfxnoah.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gyozmhghi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gmzbyjcsm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gguragrfp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/galjbseen.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gsvodltuv.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gkkyozlrk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gzpxtixvo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gyftytxsa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/ghsubbuff.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gdjpiejzq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/giwduufxg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/grdfxsdkm.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gbukgekln.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gfjjdnesi.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gyyjsyksb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gothxsibh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gcjzctynu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gsvhwmyqz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gkobyvqyx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gjoqhqjgq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/goceyugdn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gphndubqc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gljdochal.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gxyuedwbg.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gnjtoikrm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/govinkrvt.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/grgqakbdx.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gizpzjjkp.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/grwowagsr.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gxcsijjjl.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gykwlsaho.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gtfpblzjs.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gwyieiybp.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/guihmivbz.sHtML


<!-- 参考信息 -->