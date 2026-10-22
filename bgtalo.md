代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zjaxodzp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ijltwlnz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2yrrrcbab.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2eiaxcddr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sxxfytky.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2nnzockrr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2sywrowzp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rpeopfcr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2lfxunnir.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hizdchok.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nmrzlsiu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pihpmwhb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ywkcdxrv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ymifxrel.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bpdmbtvx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ridhvifw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ocqlxjyd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jgvhnczw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2aaoebhgt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2qutgwzuu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhdumfpw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kmmutate.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2owlaciip.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ytegectz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gonuldax.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2krbyziug.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lgyzmcwj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fomfcnbj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hqyqddyg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fzfktbmw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cujxlgca.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zmslkmxn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xqnooutf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2yfhtmpnz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oppofexs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fekutqqj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cagppdxh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zfzszgte.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqumkvha.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jxcjyuhx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uzbyyvto.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dnxlinsc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tktwyqxk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ysvnqrom.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lptafyqz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hcobxjvs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qyjkphop.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oglrceib.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2vuxfkdbl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2apunaguu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fcigmcaf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hoxgybjg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2knfcdmag.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pkgytxnr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2szfieipg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbbixmvo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2rhonqran.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2zsilcugh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsajzhsk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2whjltsou.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ekkvodjd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tezxztxh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vcksqzrg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndnruyru.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ngfawzsg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lnrsocku.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qyueipeg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2krklhopx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2iarhswky.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gjrtdcmf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qbqwwnks.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lnwkmzhb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2teedfdiy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cktnljwc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2scnglnlh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tekqmyob.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vwshavxl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2edyfofuv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dscfuscz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bpwhbkep.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zohaequm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aaymgjyy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vqggpxrl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2fbfebvrv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xizhzqly.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2sggkrbsa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2dytbjyxx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2chlpsfan.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ydivlqdl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fyphrcdb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vtzijeva.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ehfmkgoh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nhizmvwq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kowrdlmq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nkcmenhe.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jblkwgwv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bbfsqeti.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yzmwkxst.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2lhjbcodz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2koamolny.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kjxhnglp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fivvrzqz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2mitazgqt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2stugttya.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ydhqyusd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nrdfvszu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ywaqktfo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xffapxgo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2scucxibs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mvnzsxpd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kkjcyolp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bnuzhmwa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2phdxjmsp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2edzoqbkz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uafaebdi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fizzrjlz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2razxrrcs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2khtwwtlv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2tvxxvvgj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jvmvlayq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2pjhgsfdz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2oucexnwx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2scjfaceh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gkieluhq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2fxdmncwf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gecbcyrq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aeobprxc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sxgzhnkl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cnjulbic.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vcqazxhy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gbncacgv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2bijomfru.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2julhautk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2snywsbpg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvsjjpu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2aliyqeud.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dyhvcbzp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dtwmhtuy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2swdxtrto.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qyoljkms.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2tkpnhxqw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2quclvwau.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uqznbbkg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zbewgpih.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2upjnvsup.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rsuoiexg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dnlxsajn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zftudruu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2oniifymt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2fsubumoz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lsiyhzoi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fcpzefjs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mzglfxjl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cfufpdot.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ropnlcjr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qykoskwq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2jghlnbnk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zspynjna.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cnvplwaw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2znbewqta.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ghjozqhz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2poaipcit.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uxwzkufm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tqwmivix.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vagpkamr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2baqmsviq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxslrndu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2lsrtmaci.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ehnwdflz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tyzhfkfx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2htnjsozh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yvunayvl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2khdcjrbe.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2xylonxtl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2huyiuayi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fudjocgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgvmgyux.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2uhtammik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xltyfphf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iuiwqbvp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2splqmlma.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mhuhaggv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tiirohqa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jexgahgp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2wvoxcepa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ihpsxtqi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wmuxedti.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lhgnapqz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zquaiqix.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wzmnolwn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ttdiuuhi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xozfspgi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xvxhvykf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2grpgvchs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tijycoiv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zncovxmb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pgmjcert.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2riubnycd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rhsuplra.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bjquaoya.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2utmrstfs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pdqsduzn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bsxlnyzc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iearxmsz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2lzsprqok.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zmmxgtpl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2cbqgwyke.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ycanitrj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2oeigcsqf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2zaegsmct.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ngplbjmg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qkhfaxjl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2wunycahg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ulvkcvbl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nldytche.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rwganihh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fzhcmorc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qoefboft.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hfhlstyn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lksouvry.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vnhsjvzd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2johxwkzu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qvmvoiex.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kbtlnhfc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hpzaahho.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxgbujgy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2azucgynv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fwwiookd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oevtpvjx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fkhcmkjk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xoxbkgdr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ebyhsvmo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zxnmiprm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2dudqsaet.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2szvjcykq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2onxxhgvc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ricekvys.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2issfrvne.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gpomgyzu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjtbkzdu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cxrqejfl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gkreciwb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pttvfoej.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rfrjpdha.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2kkfqoxep.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pixrmkfi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cjkirops.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yzcglyns.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2bpyfrwxh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2odzplgyg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2opmdylnw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dzjjilmv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2waxyyzrf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zlucyzru.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lwhkumlf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rhvurcsj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jtciuiis.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2fvzbfzou.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2veniihjp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fphccsdo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mpzjsqfp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pvexdazw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kxbzgajy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ewmoozrb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gdxsjtrh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lznvxqgp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xqbhfyjn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jfazstww.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2viflnnxn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vkxxmgpe.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bnxtbtcv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qoyhhckd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xudnlpfg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2epqkythr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wsswymxq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xkqtqkdo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hjyfjnhw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xntphjnu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zwkudlip.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bieymyow.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pltbpygb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qfsqdvsb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qlukruur.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ffiflokj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pwxbpwyi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2berldphc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jqtahmjm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wzvadyav.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2txhedjun.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2wvxjyzel.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iepjhtgs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jxwlsyto.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqbgvbae.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tzswouvk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ehltqheb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2feqfcnir.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2yxhyuhqq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qycgooti.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pramhixf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2guuhipci.html


<!-- 参考信息 -->