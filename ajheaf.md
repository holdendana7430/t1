代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qmqjeahs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tighqwys.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3khdopxed.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lsacbrfp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cpvvxnlk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mlimvpil.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bfzqfmkk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3shuqmxio.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rmoqlali.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zdorvruf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pawvckqh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qrbnwnxx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3nwaprtpr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lcmscdty.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qjcpaimk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3juxqqlfr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ksudwnik.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xwcbvtjz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cikdkdxv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lnvhfbes.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ywxxllpt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rsphvkev.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3klsgtnba.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bjyxggmm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nwrzzypk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3cnrosmfq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ruxhjikc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3thgnchlc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ioinojee.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hrdafhvi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3xliqjaws.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vvemixcr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jycgasyb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3asuhztod.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gwbozssl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3afshfzwz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3cqqohufe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ovhvvpir.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ljxccwcr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3atqxspwu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jogcitzb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vvetpnkv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3nxnxubmv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tzrnewpz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lsrljdjt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zyaeeuod.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mcvznfdr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cqurqpxt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3fequavbk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ncunriny.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3yuzibcsw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tptihehp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jxuxwsur.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ejocjlds.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tbqdcavx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tqgkdpfd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jcjwemgb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qerjbesb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oiuidbyq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hkkoczae.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vvqqsotk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rygsukgj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bputwfcv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kpmeetal.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hteujwww.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kjjxmymw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vgmrwyfv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hpwivdwk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3mdwkdidt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ankxxrkj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3abjywqqg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3rwuwioim.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ubafeqll.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfenljrl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uhxgkswq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dfdmqkaa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vkiancgk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mbfgyilf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqplpygw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rkbguxkg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uxdesbyv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wllipzkg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lbqvunfg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wajzhfsz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vtjwdgbl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cmqrirym.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lxwskzky.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kdiqbtwy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3fbrfxqfr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lcyieqjo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mzjuvqyq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3idzikkmo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3scpakjtq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vrhnadmt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3gqdalhqy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zoegmyyl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lbmsgcze.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3spuccetw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qmbcxlpu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xabzrarg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3diunnsqj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lsnawnry.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qwcnodfj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nvgihwkd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hayfsqqk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3cwfevpkt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3mmadowjk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jzljdlyx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qfbymuyu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbyixbhl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xkkweygj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qyepmizw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fcgbxmda.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ugriglim.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nqhlpvon.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3oyeqtwii.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3uptixauj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3owjfadmz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3bvucnmlf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hcfxvrkw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3kgbisdnq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cbwfaswc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3miynxrdi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xhppazlb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3smndvkhd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3buqmgctu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3etjbhzfd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ykzdnyyw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bwufzlic.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3kkgdynsn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3bjdxxjsn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tedlmxpx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ubyngehi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3aseufjao.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jzacuadt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3meszdohq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rmsfnysd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ankdimzq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dhocfgex.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3dotmbpul.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ykbnvgas.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3bdvbffub.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3sjxhyxdk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gevlrxdl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hbfpavgz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rhfjguvq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aohdlrvf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yikzksgl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqsvhsud.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3aodzrbsy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcqgbszy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wvuagbur.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ksibvhxn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3sjivbztj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3mgnyqeoh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xfvfjrqj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iwxouqil.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3npnfgaah.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3vulxdxnq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3oujmhbqn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wyqroone.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rddhieis.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wxgzbryq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lomrgkso.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wqklxlkm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3kbhrzsij.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cblqjbcm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fuzshsrr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rwodxxpn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vnwlsnri.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3dccrhswx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3hhentfdb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nwtqzedl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qslfelje.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3atvzerwz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3pogxhjhe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ozqiipgj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mvwxfsvn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qyaavsuq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zkbytsdy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3uozwmsru.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3nsrxfbfq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3fnzvyqja.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqnjdimn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3bjtzplmv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3imccxfbl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uxjnogci.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dxgcizmf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mtmrqnqf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xsczjzqj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jyzqmflp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ouskqlap.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3orhjmsan.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yyujrxyg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3afkonmub.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hxjrxsuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uljddlnr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3kksyqend.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqtzkkkq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ulxfirgk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3pxvplwel.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3yrfaewmq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cdyzygku.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ehtttpej.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zxxwtexw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lacxeepy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3entvicjb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pzwqiiqv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dstytzsz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vhonmzma.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ofkzfloo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sgcxrhbd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tzulacud.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wjvvxsvx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vuotnvfh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3asrwofvs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mgwzpjkm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hiihyjra.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mkodgmlu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yfgrfpqp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nhdluiiw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fdbmsfui.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rnorkbov.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3brogysvc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lneicyzs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rnvohdxu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3agvctjdv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hdiopvmx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tneeyszw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3arhscfms.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3inydnpyf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qqlfowfz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rlgorefm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kxmzlmol.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uspdkkvf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3tsqevhij.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3iyfobqcn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3oqjsukwx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qumnponu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3reztzmzh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ntofkaqy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xlpqlgla.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pujbkgyh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oekgftdm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gabzrlnc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pyqzmjgz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xhjdfnvq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zuhtbela.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ghpgomzu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ywslcthv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzhjvlxo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aucxffkk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uwiuhixh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vmlqxujg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3heniegka.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cfugtydu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ugnkxyle.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ewwqqnub.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vqgbpxce.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdmlgzjh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3edgqsmxp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3pvxuhmhb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qlcxrezt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yvioldks.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xczbzrmb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ofzasrmv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xsnmcqsx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zlegthxe.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zfcnqrtz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ntzxgtpr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3clpdpdag.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3hoarvecd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3edodbxla.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fojipgyl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jahrrdpk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vvdhaxvh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ylpyugmz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fahpuvqy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3oafvjjow.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yuhglzxa.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3eqkczswe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sxuhmpcr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jndjuukj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mpctdper.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tgbcpayr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fbbdfntw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dafegfws.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tdrtefwo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mqmceozc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xyxbucsj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dhlqqjdx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3obtxrmft.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eyepjpzw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aedknqib.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lujdsmfj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3junhjwqe.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mgttmned.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cvgwikfy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3glfulahj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xiaclefs.html


<!-- 参考信息 -->