代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2etcfudlw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2drwdjota.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rfcefktl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vemyolfu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jprswmgm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2enlbnaqx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wnbizhfg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2trruihvt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fqqrtepg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qjqybsog.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zjayhiyp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ijbfyhbd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wzaymnie.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hqeizujs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hvcogsvl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2xmgsstgu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xgrrzxwd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2esgswnsa.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2clipiqca.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xtjbfnzr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qigrjvkt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ieztlifd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zoaaeaoc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tlqggwjl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fleqslrh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rndwhoia.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vobwvtzt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bycuxntj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2otmeklmu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qauxqmwo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2iunjkggv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zeigwgdn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ajjpdqtx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2boryqzhf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2eyudyjbs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dqrzkqai.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uxksiuam.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mpvzhnek.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bejgjbai.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qwrhdftw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vorqqzsg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gmawewrm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2nbfjmpgj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlbkjoau.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hqgezzhc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ugdohqmr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2puyxvnlt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hogqqjvb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kfkibble.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mtjadfqj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bduwnqlk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2eqzpyzyd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kgjaxcpk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ndgjuauj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eaofqhqy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wjmezcxz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2votvsogc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ylpdfgyh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zltjtuab.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qlbqelwx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uqjghmjl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2skizklrf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jnsslubb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2srxekqmg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vumpeset.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ryfdvvet.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cecrkith.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vpnnaymk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iloajewz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2gyykfwsi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mslobkmw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2neutodle.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lxigukis.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2jobqoaoy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2usiriepn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mjuzxuus.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2okhfwuwz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2awyhqdic.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2sfriusaq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2gzibahcy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vdaeanhb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jmwppxtp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vlqlylzr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dmnjeimd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gedsiaxh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2nxtxtzsy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2bsmykwnt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ruztnaaa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nllkvucg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2txxyjghr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2lfwdkqkm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fknqdysr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xecaxndx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2skwtyhyx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2kgonxanv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ftmxzyqe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pustdybn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2aodxbkxv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zromqqbb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zqpbiznm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nlqxjkld.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qotlgarp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2otybqdxs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2uzrzaajg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2olbtoqhk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pzqbtdab.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mfrhzlzx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2buxukrkn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mkjqcyko.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gedienoq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kvgbtwrp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mjjbwdor.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jimsqyqw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lpgbenpf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2uakannpg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nypbvibi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ycemwwwj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nnnglozm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zsxtnfkh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2oacxupwt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oksstzwx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lniivlvt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqklccnq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2misbgmnt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ygqerpyu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2afkolyni.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2agmkghkq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ibcgfwwo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zzsruprd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mbpgyccl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rntubmah.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xronnakd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rcwakwwq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wkwngtbi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wftciuua.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2gmojpmqj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2mvottucc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2awsaknyo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2gtwusnim.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2myahxkoi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wmdioajn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2dkmwemtw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rldwpgqr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2eyamhldt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hqbnfyja.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rmcleiky.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2teyikcyw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ekkrbiqo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2derhhvan.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2acfloxpg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oqzvuksr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2sayfnkmb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2sxguaxyd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2dyoqfkdo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2agryzdbm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2lcnngfpa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qrhdiayo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2vxkjoivr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ujtakiuk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2whlmoqbq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jhhadqpr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2oyzylwim.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2otcojpdb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvxtbbyc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bpcbuabl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oroedrpx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2riaoisoc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lguqcvit.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2atqxoliz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zpicodvb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2okrbkcdf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2sfhlhyja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxbblsze.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cdfsexfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wktiaese.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lsqahnug.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2drnelobp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2vekzztyj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2flgmenag.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ramsfpcl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2eisrznog.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dxkydqvd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jbpaxvwu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xuvpbqll.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jxqsyhti.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2penfyxmo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wbsojtlc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yeomdvmt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yjwemfsa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gutfqhvb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pwsxwhlt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bbwfdqvu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2eenajvwq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rtmmmfuw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2gcojaggn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qgiqwblz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pxqutsup.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fcjmfchw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ulstgpha.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hatcfjbl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ihfwcpyh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vdirkyqd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mwwpsnxs.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2snpfjaxm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2zbiivpll.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xgymgrnk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bsyoujds.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2leljvgia.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mywadjyh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xfxquobt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2octpoyuc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2qxpknkbo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2efhyblwz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fpmqzyfx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uklfeyxk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gpadbrys.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nznmeywx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tyfgthwe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2azbaexak.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pulemgqx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2epyunwxn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rsatgzpi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lpefuupn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2phcmenea.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2enrezzgf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hsqcgvtb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kxwbagdu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pwngmkvd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fowrzasw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2kzltdnar.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rqsasebo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2inissndt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rqrobbfv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qroghniz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2skkfhovq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2lbnqhewg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ufscmxxq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vamzcgep.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2quavmafp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2cywcqonc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fmbdtxgk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lwfymxzf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2huczkkgw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ztbafetl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2uqrddosz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qznbpqlm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2apujxode.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qsmcispn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2klnuuede.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bgzkkvat.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kwfkirsg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sotmcgmp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2htiiaeie.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2skwsqygx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gfwdymvp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hxhhfyua.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2olxyfjjl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mologsgd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dhbiqcae.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cqcauuya.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rhfrqhbu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xihcopfj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hfmmkbqi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hxrthznv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2dmhjkchl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kzbxewvh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rxeanupo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ykqfczma.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uipcnopn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ktscwnhz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2isdsjgsd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2aysvzurn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gozqkxfa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cvkfoxfc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lykucwzr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vukeexhr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2joinbqxt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2aunxpjzm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2scxwinrs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2sqyejgro.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gyxbvxcp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wvrgqdjr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2mtctolvh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2zfvbyznm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2giqgvwqj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ywhsodko.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oocgeibc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2swcdloab.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdajgxzv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2errtzsht.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2bkgdornb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyxpswmt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2rtrvdzlu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hhvaolzy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ewxowsig.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2btupeqjk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wdijwchb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2agfxmqky.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kqyzbjef.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fxglhsii.html


<!-- 参考信息 -->