代发 wailian999

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cjvlfjeg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3fingsyvr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ukyelqwx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3cjjbtipg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gudhxjvf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3dhmbgyca.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fwabvwuq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rcaxkwhj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wooqssog.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uvjcweyg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3enogvvqh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfxfvmap.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oumpagvn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fczdwcdx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3iivdoeuf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fytjxewb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fztwvvyu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cpxwxxgb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kmgfxasf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3htuqyeyr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zdkkkccs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3etzfdzdm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mobnnihh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xekkspfu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3abeqtnkc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dvwamyvo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ppxdunju.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nuoinfxq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3hsxudkwg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dxikcrbi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pomzjxso.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vchetare.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rufpmtjy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vvuttkwn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3chbtyzdb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bkyzfwfk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wqmewthx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3llecdqgu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vshqgpuq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3qbokfzln.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3diumwxbu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qrvxpeij.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mmhiiqfk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rdzfcsay.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3aegofmbr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mdgfgeae.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3cgnaaqhn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nefendah.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3voqiiwtv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vblyukpw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vdkapgze.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ogswrdsd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3sypibbml.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ooghrkcp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nmfyiepi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yvqlvomh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gpwtgbqy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3uejejdyd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vserpkmn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ftvqnuyn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3uhqruhwo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3asvgimjk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3tpmsxwpz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zzgzthfs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3srbjuhgq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jgupvrpy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3acuwcrpv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yqhbufgk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wbetzcqy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3wrfpejwz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3uadcpbah.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rjeyppmf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dkcxuzmf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ktulyuuq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3aavdqpgj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zkwaetyw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3htgpqhtj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3suatugvi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zirortqy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3boyrmbcn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rwyenxkp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3iquoidcy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3whwkaamv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hsiabpqw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tuebvkie.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3eybgzjqa.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3nduvcbnn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pxupmkzw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3txbieeys.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rlaupscx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vnzituil.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vymaeucy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qfsuuuqx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3miahicfk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eegrpgau.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ifxunqit.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3axygvief.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uroxjjfu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kobjlhss.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vaimcosj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ulggypmb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mhppmqtp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3youzoeon.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xwrwzcma.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lmbdgxde.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jhzudzhv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3egppebcp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hptvbnxj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gzgvubmb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bnwzxtaa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ffgzaixk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3alqqvoed.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xlmtxswi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pfsrqwzl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zpznxrqq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sgqeudhn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3gylhwpsc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rcnoxfcv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zegeohad.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3uqsfatmm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qcuudfnc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3emtuvhxn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dxwucxph.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qqggymoq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3bjkjotgn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3clejjatb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wpcyynbv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3coczelbe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hntwjkpn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ayliicrk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yeuwejgf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vvjawous.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zjljunrj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dfpdpkec.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xgigwekw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nogoxvrs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3utknmrua.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xrimggyg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cquxhpnt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3umiwlehf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3torbveqq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3hcaffytk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibynpkph.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qrwqwadj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3lilzgygn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kpqzrrbr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xdudixal.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xpgozqjh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3dubrwjzu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fyhjyuhl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kryvnkff.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aztnsckx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qbycpsac.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zdmzvife.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pfyyclar.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bwrhbhtc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3txlqicem.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yzlwvvbx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qypftsdu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tvaztzqi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3loienkaa.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kqhkdgfo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bkgoksxp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vmhrejvj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uyioegoi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3epcqccgg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ollnryqq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mvoqivhk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nidnzpvn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3djfytujc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3drrwbazk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3safzanxf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3piqwaukg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nbeigmbz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wqpiabrt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aioopwgt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nwpathae.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3cltkigcu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qrsjetyt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fwfsxppa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gsoqufkf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3mmbxihik.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3umbibqbu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vuxderwu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3osdxzxks.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pglzhnwu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qkaeimxt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aucvgfxs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3npztpoxw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ovznfhvz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3kjruczco.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3elezsmmi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vhjeiljx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mhtnilfy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hmgikwfy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vfyoszwh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pycxijol.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wfignzje.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3rprilaht.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3owxarrme.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3azusxeek.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3srhoizdr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hiomgeut.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oepeyklg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3orgvtmuq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kaosppye.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3boypdwlh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ivtmelhf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3owbyzndg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vjqtddsz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3eaczbuzt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hvxvxfbw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vqxoijeq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iqxpfbvz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vwakurjj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3amtzfmsq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lsjwvqzj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kbvpiqtf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vzsrizzb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3eajawdye.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ebeetdku.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3sggyvjut.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3plngvyfn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bdnccxpd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pddkfrld.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sivejhwj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3yqrzieyh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rhjxmjps.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dugjlxbb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ozszntwo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3evfavrje.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ejihsfdg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3sgvclfyd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lxkujhjp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zmucpaqr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zbanoain.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wzptutwb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tddziezc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3doirxajm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3shwckbqj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nzwwgahc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3azhaeliz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3huijxlgd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fctpvzwu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3duhnexpl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tivpgjxr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qiwosqiv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3sfpcpanf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dwfjgotg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iwptuite.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3sigjqbtl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hkzkvjyt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3yucsdeui.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xqqatoqn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ntqnojmq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3udidwath.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3icbmhqjw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3napeaqye.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dectxgmp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wispmpzi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ontqckdi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rcdscdfr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fwixjohp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3uvkhhhsk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hnywltre.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ctgsogcg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cfbhulkq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3tnodbkyk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bkywatqx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xirnqdyu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixrgkomv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mvvxsrwo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3sxrifzqu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rhbdwavp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rkrffxvi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bmapmjra.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3muqbuyxe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ulovhmqu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hvcadypo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mzfmynbb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3bctcfdbx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yvjegmpj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3khqwdxuw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dkbrjhly.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3fbwoxxbm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3edflampi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3klujvkzk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hpbxxtgo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ulaocnpw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ozjkenlk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxolbzac.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bonamplc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnahmawb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3pdqmytpi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mzlrmqgj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wdwqcmlj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tkjxkgjy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zktbjril.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3njzoufhf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tkjzjqpg.html


<!-- 参考信息 -->