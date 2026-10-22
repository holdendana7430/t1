代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jmoxxiwn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2udqwkuvl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pbacagky.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2swbjztlk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2bzbsmguf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fhzqxwwt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gvravuev.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ffumkfms.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xltvxtwx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2tacmlnut.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mutdrlog.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zitfxkvm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zsddpnah.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ygegtsoe.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2opujxeiv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2frmeqnbr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tvuapqls.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ygrtouri.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wdzkbsoy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2icupoivw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ixbknynt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zpjjqbch.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ynfcgspb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2deopeflv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zdwridfs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oejkuayt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xspsaqjr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2udbxreoq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xopulwis.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hvqopkjx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ejvtnxff.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wctkfvre.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rtylncmx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yvjjbfvy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2khgmjjfd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqoztcak.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kooyhndb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gzrmcygl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kkppsvuq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sddotrgf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xldwiuqh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vgqtdddi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ihuzhcqr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oyajzmbl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uphbqtnm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2hdzwwbnt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xmqpeiog.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2unjdjdme.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xmkjwpuc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2covrkges.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bhowfowe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ctsznfij.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hkolgofc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vchsthdf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gribufdm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cfxzahrs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bgyhqiem.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jemajjwh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2aejssgha.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2amstpjsl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vryppzhi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2koxqlbkg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lewcaxur.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zcyxxiuc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qliywbbn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bcqeuikn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gujkauio.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vejoqnjo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ygfzbmmr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2wdajueap.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wpvmthvq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xieamevx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rmufqdou.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gsyalzls.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2oexdgrxp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iluizilv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pisodcgj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qwhpgzlh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2abuboncx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qbqdyued.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zkdyshtm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vulafdwi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wpicfoog.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2necepkon.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2tpimankd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mzgkfhpu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oerexdjx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hammvzwd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wtzoldcq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gukguibs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ckszmiqx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2mvgboomn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dahlypli.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2rgqddrpv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2bprsatjw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hizhlslu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2kitczlvz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qkpmexgy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2khfgwlvh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pfrpjlvw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ltkootro.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vnwsumoa.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pibawmky.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2azynhzpf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2odndcpmi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kjlbvyum.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jrqbidmh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2quaebvdy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zmiknmkm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2njkqzbyz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2dfrpvrmd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ioqacfrk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2xkpmdvvl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jttjzsyz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mwcjjvat.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fwaavigb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zcuyowku.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2rivezrwc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qbnnfnlq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2atgjfxhs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fsanmfsx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2gaqboyps.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2gdibokwl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pggqvqgw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2dnhgklxj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ezdzcfpk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2azivancj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ajghkexk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fyenwkwo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2humqicvz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xsyeuowq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ewwvlthd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2adzjuyto.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ytaajlll.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2apnuoxsu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjxtvzhs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2dulolcyt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqnaerrt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2epmtnjcg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hsdevfrz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tzcgnytk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2psbelzlc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ecgseagr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ahusazac.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mavnwqdu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zxyomykb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tttvuref.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqqwmkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rocdarhk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jeajdfpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsdyjxro.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tiilchhk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wwjswypw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2incgjyes.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mmsmvvie.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cilvaeve.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xubrwxno.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hvucbghb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zxjjsnqo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ahrpjhll.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fcneibxi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vnmdakta.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dhqazzxt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ggchrhcj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xsxkyozn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ribevtul.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2akaiewnk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nniggcyx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wwyutlgj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vpzyvigr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2cwzasjbt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fijjeyvq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zqtpdcwg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2adnfihsm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mubnhfrw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wvuutfpz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2thtwjlrv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xhbfwuub.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rbncztvx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kugegark.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kyqpffbh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2pamsuser.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zhpwmdnr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wuqjdgdh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ziudbrks.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qwgmcels.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zympsenp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2vjbtbvwh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2rvgrpbcj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jywpczic.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mfcsrnha.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pyzgfsxa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2perqlttd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2abyyjzmv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2azgwwbum.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mlidbwlt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2yolldffs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2idsjowvy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2thlbpayf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zagplvxe.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wycewrjv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gpjrdmeo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xckxdfrx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ewjbokdz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cycigvkw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2llcvvryx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2wuifazoc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zkfjsato.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ngkdvfwa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eoidkkrp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mjulidwf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozghurqx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jmrqshjc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2irldkjbs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xsnjijmr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ajltjwjl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2falkoddx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xhrtqcqb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gdttnewx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxwqdiy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2tyfaqiyf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2usutxakf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bybqvzmd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2dluxgxpl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxfjzqef.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdehzprm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qqzfcdtp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cgheoywx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2emjyqkrx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ndlituan.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dyenxsxi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2suvwijws.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2sxwufdmx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hipsetie.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gednmklq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mbrounue.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xggylkme.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qorcnolc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nxmcmtkp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kmxbiabf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2dziwnlce.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pvjukwtm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ijkehinz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ujakrjmv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2igcbnoxt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pfujgaje.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hlupwohl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2deeneucs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xmpqmlpt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zilbbvxn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kmjypxrj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bqlolgwf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bxvqhtmd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2elyqqajs.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fpvjntco.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2emoijyta.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2idljejye.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2joknidwa.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2kzmfkiwu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2objcnxhb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2axlmdyto.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2fffskyed.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rwzvhdfx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqbsjmcz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkwqcmsj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wyldnyam.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pygnbzan.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxjlaaqj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rkgpdqkk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ulzwmeyt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fvlqtvkf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgscrdc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fcpmxhse.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2clayklwq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ksohshxm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2swqplxrt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wjpqwskk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jgyjdllg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jagajqfj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lhvwusec.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2jqjhaajc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aszijwbk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pvbkcdkp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfejpjrp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2riursuul.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fbnlmrct.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pxbrslxd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2klgctmjt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ntzkcnsw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qqxihhmy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hhkspfcn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mmzwskts.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2iswguxsb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xfpxeltz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zedophjo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kyqcajyy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rzarvhet.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdtnckny.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ppmsuqpt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2isfovakn.html


<!-- 参考信息 -->