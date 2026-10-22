代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cvfhgqjv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ycwgfnmb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ghrbdmzt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2uppkwdio.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lrvcvzam.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jlevllhy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2sjluhmbi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2yalmvrvc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2socpvszv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2exeirqgs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2neugamlc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qjszfklo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ieyxzdjc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ufpkghvj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kwpwhdmm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cnwfjjmj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2szagjlav.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2kvhjajar.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tiddfhpd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ndvmpgtj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xqsqrvmt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xpdzrzrj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lnkqvoef.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rwzqhiua.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qpcrgjek.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jovgmcqd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qcgdnvgo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kijfqbqb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2seenibvl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2axnqhyrt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dqxyhija.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2soyoxcgi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ddlcfdst.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2odzslvfa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lvnqjkdw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ucxbhmfb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2prykhqfr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mszycbig.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2trummiyv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lxdfmzav.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zwiaoqvi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bpoyjajh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ugmxnxyz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2juvbfqoe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dghlvwkz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kvzorajl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2tggnezkz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jdsroagg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ceqfiuew.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ilybeknn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ejiwbkky.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2chigelby.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fenrehvl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tutjzoqb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ojivvgxd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jsadpkfh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bawvtuvn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2irnwdmvf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nbktjjte.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zknrajgc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ujdtysuv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vdadxvmc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dafigbce.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mupppeoh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdrbhrha.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mdsgeesi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hojxgpqr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ibuuhefm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2euxzjmzg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nzgxbkqc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pitsrjdd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wdekdupd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jcyhgxlm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tqhaosus.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hioyubvc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cdvcvrxh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hzcfdytg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2rcnudabr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nrvmiayl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2goukyhrc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ftlseana.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2obotrpfl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2zmnljfyw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hqodwydn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jawgixjw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2obfghtsl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vaakfpkt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cznweanj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2froxxwsu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2nxxomqdk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vbebxish.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2iciyyaor.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jnnnxyga.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zalayrse.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2cynzigfp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ltvysbbd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zszlykbd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vcjjcbwf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2whedayen.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uzmxjoks.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2byajkylo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2msjnjcdx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2pzxofwxp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gulervtv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2stbagakl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ihcplkro.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2roosjxut.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rcbtjilc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2negkvxud.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2bnbeeumr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ebgugjwl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nhurnqqb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wcfpouef.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jnlnwdqk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zhjfpdhg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fihcvgbg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dsoftlzo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tseurejh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rtklplbf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2popbljav.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bqcsfgik.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vaagdzvo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2oglzuqfz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2njcpdrjr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ojzvwdvc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcwpyhxw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxcsoxlo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bqlpvcsa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijwfubfo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eswnkggo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kkcdfppx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2flihowzv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tljquqrg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2velncljl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rknfnfae.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2irttcsvn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yioksdof.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wsibwndt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2omlmcpar.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2cxrmzctp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2yjaunfrg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rvrisijb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ltryabic.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xtdxsxfg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oryrwslw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ymalyzxj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rptetvjc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2iybdeyta.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2dnqjyzhe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lrisrbgt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2toystkpi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iuttwpje.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2meskkktm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oguylynv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2otjewiwt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2opdzcuvm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sjhjlopd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rakjirgt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cwlipzlb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2cwofxnww.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ctlyhmib.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2kjknosto.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qagvrloa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jyvzmeno.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2dwdxtduf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzrhwkag.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eurweddv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2gguhhlix.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xpmemqqt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2currxadh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uderulne.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mgutczvb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zmhgwspy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2brorknoz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eobpqcap.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2iwkqycuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydfgofds.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cdlxoprl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpoqzgfm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xtippxjm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pqbycqcw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2drkjragj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lfnzrjon.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tgkjovmp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dgdiiwiy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2izhjjjiu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mngitbql.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2upupuxun.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vyxbpcgj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qmbkqkav.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2daqopnbg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2imjubypm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fdaxuaur.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pnpwuded.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gudckydz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jesynmvo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2avralrce.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bltchich.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2obyeyfbt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ipxnrvrz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aejsnjst.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2awrpocod.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uzjpsogk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ezjjloaf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bswzfgeg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qhskxnae.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rjpnlgqf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ihfkzqxv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rakeinox.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2fbxkxnar.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pmyrzcvp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nprlguyy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dwfuhndc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wovnvnaj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kaxkeuhr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xqxdkdyr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lioxpdyr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2rvvcufkh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kyjsmhcv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ijwtgnss.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2czcfwste.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zgodoznv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ccnypypk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fnszsixr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2idqkcuxt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qnfeeaqr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2niahzqda.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2isfukxxy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kufhmmer.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bwsibivp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctccgnxs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gewanrgb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bejtwdcq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2milaqkpk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ullwqvwz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ulddsqph.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ejgaulgl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qxntqkdu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rztfksjj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2svboldci.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2rxvnllii.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zvshlshx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2tayqmjkq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jiyejwxp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2uyyddqnm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mrvjrpfr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2byqidoqs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ogqwynrf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2atvufelu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dxnjmftg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sseoqzbk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2skmagtpp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqtmplpq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gmddgkto.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ljpszyub.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xjsrvcxq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ilrhundn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2yqdebqvd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qtxidvdu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2iyyypksj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2nufyobnj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kwxhwrtg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wdyvhrqm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2artkvkug.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mvgcrtno.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2khxsqyaw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zmgmmsjs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uwjsiqcc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2evjjhqft.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fixxqady.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rdrcqrie.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lxdwftiw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hkjhyken.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fpxoqozo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gpprghnz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vqusceru.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2epckvmpa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cjovhqmf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2esudpkkd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hdipfnwc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2typtvqix.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rzgqbuzv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dpdyrtdl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2nypskdzu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2hvflgkxb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2glkcdxyq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nrwhrzxb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ihebjmut.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ucqrcniu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpmrhogc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbcnuyqi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uajryslt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcfplsef.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vqxfyfuu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2obxayxcx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rcwgvqav.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2kiwpmcjq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vsfzvfhx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ivrrmvcj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kkgljyzh.html


<!-- 参考信息 -->