代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tiwxxwer.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pudijsnz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2dkjobywy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2pbfbdrho.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xlpzkmnl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2bxfeztdy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vuuhpuyr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2tqbfylzm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2kincvoec.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nmqbqbtk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nogywvlp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2rnmfpawd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jssmhrns.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lgackvxx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gvvsfedg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xjvoumoj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2xnjikkjc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2bpnexrxb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2uifemlbg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dauxejfg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2moivjuoq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ufazkuzg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2wrwgntlw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2kihicrri.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2reopgirm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lzbgpxtt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jetjjxbg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fdjjhsbw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hsdhmckp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mgackibm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qedrrthc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hzbkmbye.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xhvuzysy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2dgixzoag.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vkdyefos.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2weabnczt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2kgpulmta.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ehjlberw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2drusjykj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hgmfrsnt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xyosdivu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2smjbjsis.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lvysouha.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zpmdgxcx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ryxzvhka.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nfumibdo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2iwxxobtx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdeehejp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2amcmjdik.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ignjslgw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2abusdgdu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hbdktiub.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pxgwdytf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2imhfrfyp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cwsynian.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2muybjpjz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2wtibehkq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dvoxkycg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tyqdolqh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tcffozwq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qlntfeve.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2riuywrly.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2szlkxess.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kzxnleyk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2migwnwlf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tzilvecj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pasiuewl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jkcjhrwy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2iivqjzdt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xkmyigab.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2sfudvmvj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bixvgiss.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xqlftakl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2donlyoqp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2klcfzgtr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2yobvxgpq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2atxajwvy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2rsskootv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fpqxskxo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mkkjsott.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hivemmom.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tufujwgb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2uclzytke.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2mukczbvw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2boiaqthf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wcigtbql.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ltuatbnf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lpihrccy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qreqdddt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2uqvpbfde.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hliicsfx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2phmmwaxt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fygabcfe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2djzzevpg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ggxssmjt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2bdgywfks.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xvdhrukg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tgqqzxap.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ejcklyke.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2rcyospce.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zwonwjcs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jrervezz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pnvnxurf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dldyamew.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jojmxupe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ankfbsrd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lctilnqu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qcrokbvv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2muvytkvn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2julxurci.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2kfgkqpbt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2shqgqcwf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2uqseuirm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rbxlwrwh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vtcisgen.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pwcdusru.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zafnenxd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ewonbxdz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cwyujxwq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vhwdeghd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2uwtscfik.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ompjkeat.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2hqtmzsdj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zomontxq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fvdmvsxl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zioyyknn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kynogogn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vwdwknmd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2peibpgsh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gssxqxsw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybmucnsi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2nbmtzvjz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2deptyasb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ezmqnhha.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kkjxleps.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nmegvqwo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2kyusyyeh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2oolfruij.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nfhrzihy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2vkmebkpl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2reqcqdtb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pwbgbjpu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gezgdjod.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ijeypxda.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yhzilgqq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xnukddaa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2czaeaeow.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zygkybha.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ewilumls.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2bosqjnev.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rrsggioc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ofhywiae.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xhylccgz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hxxdrjvr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ggscgrub.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mhwletcn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mrelbtvk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vjdoznmk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2wxtwpeby.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2faxqnjen.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gbemdfoa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2vqfppwrt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qrgpjpmm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vybsarqv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2humyfqog.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kxbhhecp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2reaysevv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2achdhvms.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gdgxmbcj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wanbjjhz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2glcumrfg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jwszkbvn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mgcrertj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zyhxtglg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rmfgadew.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ejggymau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmoadiqe.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2koakgtgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhkbwquc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xnsghrrq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2skrgfzmz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2vntlyvni.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ibecuuxu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hlzznfhj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2eeidgyrl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2buhyebcy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2tbuhizss.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tfjzerwn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gnhshjsx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kwblwoae.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gdclsuno.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uimmibux.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fitxbpqz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fnyvctvd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2opdutanq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hjuqfhol.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2whrqerpq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xdrmshew.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2rthhknsz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pugegpjx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vrlqkvow.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sbndbuyz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jsyhzsgr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2waenrpko.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fffzgwnv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zlkqsltw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2oqojfsll.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rivziilk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2klonjnkn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2gscthrbu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zquhaybn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iatxzddr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2amwlmuxj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mzqtaens.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mphzgpih.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bljrojke.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kgfsibry.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2harjbkke.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2makzilvw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xpwpquyq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kgfqedgy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2kuyivcbz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mualbbrs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vmwovumw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2eufweezt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wwrvmwgo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2czycilcj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ltwyegoj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2slbimnlm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aspvodrg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qedumsci.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tpqumlto.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gkvrnwcg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kyspebkm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ulhldzpp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qvylfgbf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lmyxcpzl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kvanvwzk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2oavercah.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xegdmdff.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2avvkprog.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2dquxddgs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ysiopirm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ijsahylc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2kuyoqxwp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rbzqfkzz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lmcrfwpq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mkkyvlva.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2iufhrqco.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qzogbauc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wusqsvme.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rninbibh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2parwwsui.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2iqexapdm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vvmsenkh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vaelvixq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vawkvtin.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2lmhulaop.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cxcrnafj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bcxiescm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nkzslxgf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ynlwsppf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qhchtbgq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lqmbvdow.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qygkdyxt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2emcftawx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2baaycoys.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gwaiufwc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2footgmzt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2xgnsojqv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rkjcpsdi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2erugoype.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tplfhjrg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2turzfzej.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jfrlkngd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dtyonaim.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2anjjwhue.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dfjemycb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2srkgamme.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ypivteav.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zizyiezw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mcccyqbl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vhugysnh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qyhucixo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qdqgszfi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kiqtqqqm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2uhwyaaeu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2emgyhgae.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2owxurpkb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhjricjo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2juadxluj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kbsrlycs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mtcmjhpr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qikmfgos.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rzmexart.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mboxtzcc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vphktjnh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2gycmmlnj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yaaqddge.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2bicpsyod.html


<!-- 参考信息 -->