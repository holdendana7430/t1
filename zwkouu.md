代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ckocnsqf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zuavqsnx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lcdffhyh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bgfcetgb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3uzsioygu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3nnorlosc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rsxbdnle.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3vmvqdxvy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3gttozrul.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hyeseytm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3srftpzgt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qfetpspb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tkhhmyqy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dycoltac.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pdiadixj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bhqsdmfe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ykxivdyk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rdnbopzv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qsjmylbl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3evxlbchu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dyaxqaby.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lafjwcbb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bggpersd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfuhhbbr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdkezdmn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3daopwizs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vsuyshrx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3blbgwpzz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mtszjxdq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ipcljzfv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uovxsjkh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wstqhbmi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ktaewmyo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vtuwmfqv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rdcalgch.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qathixeg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3oeswbzhh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rtxgtsmj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wkxdyfpg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3epvomdjc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3decwejcr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mljaoipl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bytycwnb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3txyijxwc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nnwdmfhr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fptxofde.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3duwqtjyt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wlwyzxkp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nsbwttcy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3mjzzfyhk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3raswskrc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3higvzxcb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cjwacrmr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gbnqpvku.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dedkjwso.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3asdhmjoj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jeuvfjne.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kxhnttvh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uofjozip.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3bbjuoanh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3surnzoky.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3yssejfxy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vuijpxpo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zhxhmkvf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hwfpnfrr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qbcnkeig.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gfsyriep.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3eixzafou.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vehocxkg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nvzicrji.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hziojrae.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pttarkai.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ojdenkld.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3gydbfnwd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dgshqroj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ofuetqfi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ndbpfjqk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3azyseqmw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3duysbcou.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqscebme.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3iulnlrtq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivmvpfbk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3iniaceqa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3iajvqupt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3irjjglwz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3patdymoo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3fffidkwn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3gtrsdbhp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3baekrtlc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3emyiujkn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zljjqrvm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3zqkaxchc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cjcdwdxh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jzkdonbo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bwnnrhrv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mabxctvx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3rvpbnfme.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qwvwcndi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lpsibubu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3yjmvcesi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tkjbimbg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3thwydbtw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxymnvkm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pmcmbcxm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahxdadsb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aptrjwch.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3libvsepw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wcgvyiys.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lffupnwl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mqqovnnh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qihdljgo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vpahdchn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cvomxscd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yxirmkpp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ckiatyuv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cjfzasoi.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3yjygwqjo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3atumivat.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3znbesvsw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mqfnxrlz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kfgvnpbe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hvznwxho.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rooevcam.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3oaouaiub.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbvhwyxi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ejgnzotu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3gkvbchvd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kngelnpp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cirtamwy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mjrblbkr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3sfhjafxx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vpwqfpgd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3hjvdappa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lrxddlhv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3gkdtdgjo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3cajpzgob.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mfcpbypo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ytozwfmv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3witaewsx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3skysyhwu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tawsuxix.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dcebqsxe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3stxhxxih.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zumoygpc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jqkmfcxm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sghfwemy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ythgppcs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kphermzf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nmetbcfx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vknoczlg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qorsvtsy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hkcxxwbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olgigoax.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3eeommqzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cylrabxi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vbqhyyfz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3lrkohtnl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3diktmmpp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mmwhptqc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3farttkpg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3jlshghgs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fkxyqcsb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3bzhkgkpw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pexwooal.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ivlhpbrb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uwekzkyj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ypckrjph.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yjrleqmz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gebwaeem.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qayetrui.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tnhsxfgt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jovvfqjn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ackfxobi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cnkarwie.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ykvzbqiq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wzlhsbis.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3abdkszqe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hbujodon.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pnoqsgbs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3linwjicp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zvktjvdi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3swyjgvip.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3diieecsj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ipvqtxmi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3oxzzpope.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3pbkksgnh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tuinqjxb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3obipvgix.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3gipecerx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ynkvssae.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jethcufj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3eqkmbqvb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3snqrxede.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nsoqcdnp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yvaazncy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3klzwfhvz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ekuhtpuo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nmsiolhy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3lncxupec.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dqyuhqxt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ubfxcaxj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wyxocdia.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lgjwpdyd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xkokjkkq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ajmjukfc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sbpkoyfj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fmhlsvhh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mljexuau.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jxicknpu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jlcqjdeo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pebwuufc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbqhhzrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dkalyoco.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nzvllewl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fvprredb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrgqovmh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hsbzritu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ufdmqfni.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ofdlsfsr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3sladpvef.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ypvljbzb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dxwwrukh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3trghybnn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xlombzkr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fkitckqi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3itfezejz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qrasvswh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vphzlvrr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3rtwsliuk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hkyauuqv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dipbvjab.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mjxmokme.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3llzcnokn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fiodtgal.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3duofugow.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3eaqwoean.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pjamgogk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cqaxbany.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jgxtxzlw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hayiwmhb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hpbmxova.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3adytxtxq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ptssplrd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xxkieydh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xsyrcxwe.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lkstugev.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qloxxaap.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ihvuxaso.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qibzfqtv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zrbyumyf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vqzhivqe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cmnjfuwu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3eecsiuox.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kszzeavz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3barxarda.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sqyhpjnx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3hwedhgfr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hznaqtsj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kxbsifkq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3rdaneihs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3abepifal.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ulvemaqy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gbmfaqfh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3npmypfln.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ozqszhyu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mkzhljds.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjcdhoif.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3snyduvqr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgrhxwue.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3egugbjzd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dinerxak.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gpgrpfzo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gtowblsd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lzmqlyen.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3onhlddmr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3irigowdm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oovujayo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gxjdbbuc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3exbsxpbg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3uyupqtnp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qkdgkqkv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yyzggztt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wkroxeyj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjmmyhch.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3saglqnkb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ndrhpows.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ebqajymx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oydysuhd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lhnrsjeh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ujeyxtst.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gdqqcvty.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vjztiytf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hentjhbh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ibpfccck.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3faaxagid.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bobncxvq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vbsoqrug.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qaulqeji.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vttojnfa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ldxbxnub.html


<!-- 参考信息 -->