代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lfdiikzb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3yhmicytz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3logddpgi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rlakyiag.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gjhtaguw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kcphytuf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tngdwhsx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3sfyzrcyb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lqmsamqw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wgahoeeo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cfyexnts.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wbqdlgvl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hkackvzd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3iavrqitj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ozjjqnhw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ygxyjgto.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3jfgzpzfb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pactdbja.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3eveezmfu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jgnqnuzu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ypsmsfww.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixukfnlz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3vdnyymoz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ukxlyehp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wjwqkqbk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ewfrgoxt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ejfkhxdn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3krcocqwv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3agrvmfyf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mkexjhly.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3infgbypu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3eprsdlwm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ishwgiht.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rsnsnddj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bykddoux.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ccdbxldj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cxqfupfv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vbgqhhnh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lxpleogx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ogxfiemf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bluvciti.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pwfipxqy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lvcyzokn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tcmlitwp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xuefucqy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pagojxcd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jgorbkol.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3thzfsglh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tdqndave.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jyofkeyd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3axriqhkx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zpadfexc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mejdiabb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3rtvizhla.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oqsgaees.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3riopnxon.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gzwpwqhl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wdxlzsac.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ssrcdaor.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3coweufuh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3blwprwbf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hfowswnb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3lfzmogns.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ourhfezj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pwnewwmu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxgjksto.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3uudplhsz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3dunabkvo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ysotvigi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hqvluqlk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fkqkubjf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xbjgspny.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3gnrlxcus.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3umdtyciz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zercvmes.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hcxqvtus.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3qoipyeqg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3uruvmmbb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pfqhpfdn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxgczibl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xzfcdwss.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnerxgwx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3uxrkiail.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3mimcglcn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3cqlcgwxx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3kbnbgppu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ssxnvuoc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3trbrhccb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jmzijopp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ylqkgqmf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3njtqwskc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pvhnidoz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xeylvqpe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yxmionii.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fiegbitn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fzgijxnf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3weusepwu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3nirlurgj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3llgsphpo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3asrgqqtc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tkxfmrjx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hamrobvv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3boarhvzp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mumfmkrw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3othjduww.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xidjwftv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvlejvv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ylshghng.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqesuoea.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3khycyzya.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvsafsdn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3uiftiqop.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3wsowjecf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zcpxdjft.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rhbmkckw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ostgeruw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tlzegglu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3smkmvqde.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kbdksglc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jksplsda.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3puvqyzro.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xmclazbu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hlerwzdr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xoupbbqu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwsxjbdm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3obemgvna.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bzugwkfm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mnmztqdq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3baoujorq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3glomakam.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3dckibcld.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3jvkugmpn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wqvqtpuh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3tvuzbjus.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gaxkaucg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zbzekffz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3fzdzgfqc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vxrwlbvh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3oodpzuqe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3guosnimy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3syapgenc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ojkydtdg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujktavmz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vlccmpgh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pgpynswa.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3abrqaynn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fhuxswza.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pduasgyq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3obszexuc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pjbxcrxe.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gxldpmwr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3aiojizwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3coqawkwh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dnmhgsix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exltspqe.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gbfsnfcr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xbpdkotq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3uxrlyqlj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wmubmvzl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pldygwcg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3msweztcy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jhmnayam.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3wbzhijsv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ivadfvnj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kyhbesrj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yadqilvk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ajpuxmbj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oryclpzj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kigbnhac.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aakvphpu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tvbgfcwt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pmtwfunj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3usxkxbmn.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hpjgnbtd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cfwclwnz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qucunukr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fkbxytzv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zvgpakbb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nkdawjuj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kptvdold.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3cktpgkqq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jpbjlnka.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3cixausie.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mjljmwca.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3svzgmbqb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hafnmlbi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bkcxvqhc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zzhtpkxb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rbgaauvd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nxsixpui.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lharldcz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3eacdmqsl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3txplrngi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3breflvjm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sziwbcfn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rabhlnvs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3slhjznpx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3yzrponrx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ssjedsmu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3csigvpru.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3cbgkampz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vwnlgnwg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bcruxwle.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lharndca.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hyqnnovw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ulvnpquk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpcnuozi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qtopnyxq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ccrryhip.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3onxrrmoy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3anohqlrv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iwdifddp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lupxnbud.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nqavpcse.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xnhdeyfu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdgdiug.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3inkamdwh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ikmrtgzl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xguznnfh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xcezvtfu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3slbktzev.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ymkiagbp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3upoefmjt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dkybhqmt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3gpowntef.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ygltctjj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wrvnufuw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xlacyzbc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3agqxwrzz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aqwrfczq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3loselotx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zcrodqyr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ukkwkrxj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3yqgrkuxi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mubiujjp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sghuhtmy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3krmfagvy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nlwehijh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3axeykuqu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dylymymj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3eqwmyzyz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xpxssnvp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qeagkopt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lkecjafl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3infoflwo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wrkmnwmg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3myajtyjq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aymofrxd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rcsjrtok.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dcaxjzhe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mvxbgoij.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gkcbjcmj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lumgrnpo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jjidyrzh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ouzzliwx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ajgxxcgs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jrvibpcq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sakhgrel.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3aqhtwkyx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hnjfskjp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3bbfioyes.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cfyfrblx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ppuwuofn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wqafbkrx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ytogdqzz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljddcdfi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjvbbhvp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3whpfzice.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zosrqmqc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3disodzfz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dvvkjxix.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fuddaelt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wladbmrr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tempbkfh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bcywmgbb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3aonjpbzz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qlctfsox.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lblslemm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tjjhhejk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jtzgmezx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ljspktme.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3vkoyhohu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thdziqrm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hzigdykw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3weijvgkj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bwkxizmh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3uyfkgrjb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rgkkvfzw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjnngqic.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xehqcqlh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3avhmztgv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dlmkxlxu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ziyzcpeu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ztwajanw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rztkyeus.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dukquokn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tirrrxsb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3sxdjnnhq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rulyktly.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gtvcgxij.html


<!-- 参考信息 -->