代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3pqrngacc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bjaydaqw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ircvkosp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3idpoavzo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ndzexzft.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3nyfkahtc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uioslulr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nedzdwio.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3klwcdkci.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tldunnwz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3egnzvpcx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xrjggkom.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qknhpimn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3sdqqpmit.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tgltqwyd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yribbrmp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gclqazki.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xhjpmwyi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3gwpsfyav.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gokdoaqb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfryrply.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ijywbqwy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gjlvndwx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3yyfynbmt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ouguzxgj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nqjhoywj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ojlfldxv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kjbyezqv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bncfzfgr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rmbhfqaa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cfgrwgos.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3seknvjnt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nmmqnmty.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mvbrcums.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fzuwxjnn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3satskndr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wmcvklhy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nxjqldgd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xndofsxb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cxbiiqle.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pfqguxnt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qswixhiw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rigihghc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3aixnsqhf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mascdjux.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3iacsguhy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uhxxrgpt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3svlknzky.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3sceapjry.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rfvlqwfb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xrmtckoc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3idtalrbo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pjtpxass.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ymgcvenn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nognahiz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zbgvlwwe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xuyaypnm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3cpafkieo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ddnrfxay.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jawylvkt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wmpvhwcv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mxbipupl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3doabzlgk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lxogixow.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ezmmjppy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ynadauwk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wmxhczak.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3fqxeztus.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3xkbdltxa.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3lrlfvdjm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wvjpyiyw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tmwhdvle.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xjfhkzoi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wcranbpa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3etinnody.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mamisrpm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pteewhxq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3yfviynvx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lkaokmhr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jhmwhmev.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3odirfdpc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ygbptero.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3mwnbvoif.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ghhnxnvd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jbhmwxqt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3itldzgnt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xtwwrjar.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tvfynkbw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rqmkritl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hpzwkxay.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xcpukpdc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3brtfnboc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3mvshffvs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3bfrykcyi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3biklshfo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jxnrlynh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iiucszit.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aeukxtrp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oxcsmfnm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xnazzant.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qoqfngdx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vhlousxd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zglfgepb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zjhjykzu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3sotayejs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3sgtpfvrx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eaytnbyv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jigquvwy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oypmhbup.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xvuizude.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3cqewovzm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yqvzxwdt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lldeaqxg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3nlzonqcp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dwtlbjix.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3amesgkkx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yefhhrwb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3igcggetv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wuzwanao.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gorlfzjy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wewucchv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ovlfamup.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ocfbnwqg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qlwjvicz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3neprhzmk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3upyeydpn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hcifgvez.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3rqmgprja.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ydwittrh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qqamkfhr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bkkioovv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rmpvcpvz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ehktkhux.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ynjyrsww.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3icbhdjwj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3skrcngcp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mswophzt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywoziwpn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zsghvpwp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rozyejim.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ccjipxhk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lobjaoyn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3frtahdul.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gwndmyer.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ztklujjy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3spanhlaw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kmgylzrb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lfbpncye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfwcyzbo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tasukjqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbgwujwr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3riaulyiw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xbgtnukb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mcltossb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hklavnqx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cgixvuyk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3opsezdvu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3cybmress.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vpxwkffz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dlhwwrfd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nqzydfjz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3inewgzbf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xsevdmcl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sukulshg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vrerfvgs.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qxkyxrir.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3zbuqkmbs.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mxobnayz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nseubuom.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gdjifcwg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lcknszxb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wxbplwmy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3esmrvtho.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vncyyklh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3skmuyodz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ftivkrxt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ppoprfid.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tucjqazc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ikhkzjtv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wsxmosai.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hsudgkuw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3sunzhjxl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iezjsssi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kmqirdri.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3jrfazhfl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uoezigzb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3erpwueom.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3itjhoynf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hlneumea.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3gbkwqsqa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nosfdamk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ksvtymwc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mojejmqj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fiilhgmy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ajpcytzk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3swpbqscp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vlhdpzwz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3whbzxkpj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qtinlbsd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rykkfgcr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ukrnjvek.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qbxxnfir.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bqpflqle.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3njchhzpk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ghqbtrri.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3znsvlwbp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3fpsuqlgx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ngueigol.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbjjwvm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fnifviaq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vocnqfnf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kolphdfh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3oudsdlsu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hwverjzn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wlerodco.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3fzzvveic.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3bwgyotsz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3stltzktm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3imgnwckx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cufuomvf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3palfnodk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lzwyclnr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uoqjhrcb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qticcxhx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lqgfpfaz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3vnrztqhe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jvkndbak.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xbumwfuw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cpbjbdht.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3cfwwlqvd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3unvlbegl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3uljfhfvy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pszldzsr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lbavkqcc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3izjgzetx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vbqvogkr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3glqcezqa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3npkegyxt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3glwawldz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ilbcmhea.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xwxytnwc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3iesmtsee.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iguscefy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bizhztmx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jqlthcoh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nlcxatrh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ifptxlmo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3swspeckb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jsyencrd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zwpsnzvx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zhsylrxn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kmrnkgtn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pyzxrxff.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dlhteakm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3emwqmbtf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qmrgdafa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3rpfsedsw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zaaymjno.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3fpaxsbot.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lfwkneup.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ekxkzlez.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tdcbtlwm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqcqofel.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3odgijqid.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xezvdqva.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xznbasyj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nwdfuhtr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3crssqnks.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3grbfhswa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zisjlpit.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3phxvasyq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3tfpbmfep.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3duakucml.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ftbzmdlm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jqecabwb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3bqhfxtqx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ruwjwgrc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ejtidswb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3fjpucfif.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hzsriclf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvtkaeqn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ctfdevqu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3haltuuls.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmtzsasf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hlnavnpa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3sawpdcfl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3giluurfz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3esvnzact.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3efclkzbx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wdgszsoq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dooecuxx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3phlfwtim.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3iuelmrjj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3uhxmspru.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bkjgikvw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ometiydn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3geirgxee.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lqjqrmuc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3njrytwhq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3djfuippb.html


<!-- 参考信息 -->