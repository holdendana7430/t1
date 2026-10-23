代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qarsjnbq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ozjwjmbo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3urettbuj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3uddslmfp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ydofhmyu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3gannxxbo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwclxnyf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xiixcsoj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kglcxgmm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hcqgxeew.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xzckzgrp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3yjhurqpy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mfssjhje.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3knywzpzc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dndpztws.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vjcobgxn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqoeywed.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nenmygaz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3esejazku.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmusrixa.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ewgfhvun.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jqqzcjta.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ujmnsnzz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hqfwrmxk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3migsoycy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3odpvhnlo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xjfwymev.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3yfhccwwh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ddqjxeto.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dgvrqiwe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3meifypfx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3euzstple.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nfwhoyrv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qmnimbhq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3usojlfun.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3eezixbzb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3shczvrdn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3aawquvws.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dzhwukhv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hoqeoaur.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3gjmelveh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lfismtuc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3fublfjjw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ykkgwotp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mwlpovrx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3kijqjfni.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vkyzfwcf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3frouwjdo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tmdktiaw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rnlivsmp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hchhwjfy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gwrkvuqh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3klpgpfcm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ntaimcyu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jpgizdnw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fwxjwawz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3oqingeda.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3nlmttqse.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3delinqzm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gyhbbkwl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qizhosmt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xnuigokz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tezudvju.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3semsrlsr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nqpvolim.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3syzsccfv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3qjmiyvdb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3snnanxbx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yixvqlef.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ytsebjav.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ekucrxga.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vclfsdpm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vlbsvwbs.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jsbelrsg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qqcbbeos.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jstxlpqz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fcccvpmw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3etozzxah.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jiwpajks.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3zencfmzu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pzwfgvww.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zdazhzrg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yskwzacy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vpmmixud.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3rtzltpca.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kmcefffz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3afpjqlxo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3umampgua.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rexwzvsu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3deetdctu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nlxnyqll.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3txyafvrr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xxioeadp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3pxhlnobp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3cbvuguqw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3oezceqpd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3yipxldsn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ezefwwgr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jkkyiwib.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fiobivmm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lzyexrad.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dcbwkpjr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ofwknilp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3axxvvwdm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qhhplaoc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ewtjwesd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cneyivmt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zwdetsdu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sipvmjkn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vzlyxjdx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hewnrrbp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3imvqzrug.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bbhtvweh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3utevelhv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wzmexedd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3roembnom.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wgdqgqql.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xvcogojr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hdflockb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3aytdmnmh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ocihbxji.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zrlhdvrv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pjftftvw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3aewqpxfh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3etmccaek.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qiqhwbdx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xwfnxicv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qlnymffi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3awsapvyx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kjbcykuj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fgehaukf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3iiikibpj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pudydxht.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ryjvdnls.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3gevoveaq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbojmgzy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rujltphr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3fvhzlhsz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uennzged.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3deyhemov.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tjedppog.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gcnvpvob.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3prkbmrkb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vdqwwhjv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rgnxlvws.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jmqrrbfr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yothxfbg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3atoynevr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hplpzdiv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3kexyxahz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjfpprki.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hnryvgss.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3nqjauqzf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3juskkrce.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rucscunw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rdpfaefb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ixdkbtkf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sdqftobh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fopreieh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ekeostfk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ekeqimqd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lhnkrpfo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dawjinfs.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lhhtijpc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yfczexlr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3taynyinp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cnqyhwfa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3shsxprgr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jyrogaxf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hyqcrchl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vusaynss.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mnsduoes.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3absnowqf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xxttjjip.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3amngmtna.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mpljfvzc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3szzqyrdh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pseusgui.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cimzgqeo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tcicyvve.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ipjtsonl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qxlwzxrf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lpokkpbl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mcokmruf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3aeiawyqt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3aowsdpor.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ydnamdtg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3euoofquk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sybcwyyv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kbrpheqs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3abqyeczy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3isdflrpz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ttrrngqk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3cmltxvoe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3edypzxuy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ctqyeojv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xjxgsukw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3edpfdsra.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3huozpplz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3weqktdhv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mvdisayv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uquuhazw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3taxdpysk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gfyoegqq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mpadjydi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3uulebnfc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qngiabei.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qyfwoxkx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pmqqpvzr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eubybnfg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3woiggihd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhncrtue.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3iqwpehox.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3siiehndy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bcbhzuwp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmakieg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3egmxwfih.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wahxbqwd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dpamsjlu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xmkolcqw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wxlyuzir.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fhdfxpze.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mzydawev.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3zavleaff.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3uhrttdmv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jprfigvp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3flrgirjg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wnjqompw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3grfzympb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3oywlsmzz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nvnywvof.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mbknmdui.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3dhiyxcze.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bupynwso.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3uxurcqnc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qgxjmnql.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dqvwixsv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mdfavdqy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nunbprsb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uftglxob.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3totmdyxu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qdmkzxvx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3imsoirqa.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3unztldmb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qrlcfdut.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3scllkxvg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tfkkvxmh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bvfcyhwf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nchmiyyj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lzynujmb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fkyutbpa.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mipqpyoe.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gvbftwsg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bwpltxxh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jqreyips.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3utzsxkwp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ediggbqj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cpcbgazv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ziatpbuz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3abhipkia.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ycjmemho.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qhetamsl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qukiqgcx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwtbrvgi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iwtddbvk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lxydoruz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3whqspwji.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvcmflvd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3znmhhpqx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3mffmjgkk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3yeqsgqey.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ouipyhwk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3cfvmtqgv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gtctxhgd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3hyfutpdk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3drgzdkma.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gepnmluz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rinngsso.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xrbcskpw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aimxmjfq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3expeseio.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3innoojqv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3utiiznkl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wykvcfqg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpkmnpvr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3afxjqmte.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jaxnnivx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ltymcfek.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3oocotvqg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hgvtvntt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3thnotuzk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nyxpwxdl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hgvafrhm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3trewjjii.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3njfuzzkb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3dwwtoyuw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ycslnagg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ddaqwrdo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3udnvvmaf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fpraqcct.html


<!-- 参考信息 -->