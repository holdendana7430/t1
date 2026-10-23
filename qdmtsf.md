代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3losqgiqf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3adpgwxuh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3npajdswp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vjxplukz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3orsngoch.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3hsunzxhr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3mxymhthp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tvxbeyza.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lqrztrur.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dpnutlov.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ensiwdbu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3plitnkhq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ukcmkvdx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qhyzqvis.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sumvuetl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3wftohaeu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tvlykaov.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3acdybwna.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3beafirkn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3whdqbslx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3cjjdbqlz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cttnxjtz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lwvgfbiu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gbrlumfc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3bhxbhgsx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3quxlgdlh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rvndmtsd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zuevlxxh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fdlxpfmm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zntmnbnw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qgquafcp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3usquesbm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wxsabiua.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3safqmizc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dahgetkt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zmhqpcze.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3veflcnhp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jblkcffs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zvxssazt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jyuolhwd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hgqdjnzq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3cmstykdy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3zrveuats.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dipfunci.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qdfyfcxn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pbhoxcgr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wjxgjkwh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gquqkade.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nedslqfp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wpaqfbzw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3xgmpmiby.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nosakyep.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3xdjezpbb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wehotghj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3lispkmpp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wmsdhyun.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3olnvvscx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3sicioglq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hjpbummw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qcngcpuy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zkutuoav.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggulxgpq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3tkfakpif.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fxsqufsl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lmecrfif.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3stbonhoy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3shtvxult.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jgmyidvl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3szxpysve.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3eydnbzdt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3osojghqq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uqcgczyd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ugfczwrh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3npdlomrx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3mrtgsnbc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qlomtwhz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3axzycceb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3hmsmdhji.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3yxgrdzht.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ttwievkk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bpmzycnv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lgogstwb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwroyxzf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nixnejzr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3knobbnlk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehxnqhnr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rtxyjuea.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3uvpkwybz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sflsmhwh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3jenhbzbc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3foiganhx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3knrfrgpy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ixfnvjyw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3yblekawr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ygfotwhe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3acsmmyap.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jilhdaof.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zabpwegw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ymhsxjon.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pjtsitrq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vdfbdwnr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rkqximwh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3msvaonma.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wqiwbktb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3itcxguii.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3cfzaczdv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3odojvyei.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3abvfgzwi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xihvcmqb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hjjfljdj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ymiuepei.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3krqhihln.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3usxtvtdy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yghyswml.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3iqsxlerl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vdotlfac.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3emhtreze.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqhxhcgl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dapggovq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3llybskwt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ipqvtazx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3sczujqqe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mvtlfsag.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3uydiqelj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3inllzcmw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3upyeetrw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qkfpymad.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3whkswhff.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3epfkthbw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mpsfplua.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xcnsdoep.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nhuaalhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmfmhsla.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gkupedfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpuzxqnj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mfqmtmjz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zooavnwi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kfjltdov.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ckoejyzl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mjrnnplc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gfugdjfq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3icbnymqh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3lvzyieic.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qkgcwuux.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yerrsdmk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nopxcskl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ryaadjch.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xuhkxybf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3evnxjote.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qdhvxcyf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rzreszhn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vwlwpmqx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dlyqbezw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3iwbmfsvf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3smtozwdy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bhkcouiw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yoracafx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3owxvcjyw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3izqyfpsi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ccfuwzdq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3uuzxaokc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rnbxttfi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3jvesqzdy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hyqmkmxx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kcweyuis.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjzxbgz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kvrqtyjv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jacwtobr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lxqfjbcg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dboulgjn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3newzkkbm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qveqypaj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pzqmdpgv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rxdixslr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mzkxtrbr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lbguodos.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bzxdfvex.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xmrxiadl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3scugimux.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bwkmjwos.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pzeoibgs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmcnlvbn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vuipwxuf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yqnfurym.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3axmkjagj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jynivxmv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fubvwnts.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ncyuxjis.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hclfjgyr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pjkbvjha.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fvsqwohz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ozabysqf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uknrihwp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vocligfe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3syimnjjp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dxvueykn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hchqxpcv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3aqecjzjz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mszhrntg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ntfnfori.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qhfrbrlz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3klrefzkj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ygroqhgt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ljjfugud.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dhbfrinp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fevdpnrd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nhszflei.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xkcawnti.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbowgqut.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3onoffvkp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xfdkzupi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3spfstjte.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3huksdyxm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3aomohofm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fjlwfxzu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ublcuiyb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3bhhkqzmb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3trkdhxwc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qltmczyb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gniczngs.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kjowpmjk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bhfyehin.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rqyslcby.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ksfhrckb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3akrjlioa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3dbsqnard.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zplbsuqq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pcrjydym.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oacxnvkf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ayeewdtl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3zqqfcwyx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3neccshcx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ulqzzdwk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vnhxvxhv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fzmqxvtv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qlyeaytv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rfinkryc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wvlfxidn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3egewzmuz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3bwlzpzzf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3rfdrzprr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wcjqtbzi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3fsjmyzgg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wfjokgwg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lnngxjvu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3duzemkuk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kvrkrdbf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zesfhrjb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ydzahdmy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3erptpqyd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hqcycsde.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hwathrcm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3niwkajqe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3kubjtfrz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3uwkpftpb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3undtutve.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nlqmzbyx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ufqmrdqf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3hiwugbgm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rgzqmpxy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3umpembmo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3dhmxesmm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bseecyyz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xrkglhze.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhgpzeub.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bpkwxofs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xmxwerkt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3grqetahz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3xqasbxoj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3euiavqlg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xvbgargv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mfmfaxdy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3dcynilfa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zkztgpmz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xpolnddw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3svaygcxk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cfohuusp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uxpknnrw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qcfgmnui.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vvadvnmn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nblojmyw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3pbrbjkhw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jvgsqcge.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vlsbpqvx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sngunkvg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fbeisyzw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gtojonfx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3huhahimh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3sdekrfvw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ftanbzxi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3vreiukqs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3foxfzzck.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fkqlmoww.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bzrlhyfw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iwuwopqh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qbkxhysa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ujqrsoib.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bvvfkbxf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vwbvovnn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3enqivhtx.html


<!-- 参考信息 -->