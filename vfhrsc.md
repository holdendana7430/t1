代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ckbpzagw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zccgumwl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hcigdznb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3glmccvlm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3cmcqlxbv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jdjpeart.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3votlvgjp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tzxtimok.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bvakxkhg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3eyodxtwz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qccffaod.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3frnnhnym.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cyxlhycd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3adrjydea.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ztozqdcm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3kuzljtqh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cuymjolj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qhbyadnu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fvlquhvw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nvzprsoc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3glidelut.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pgtagafo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dovuwmvg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3upgiwyxw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xyrygxyh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zukrbeik.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qlgobomu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dfaunkmc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tgsppamh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ogfzzibq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hxezygnc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3syutylfy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zumfebpd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xrzukxos.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fonxkbmi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hbhjwuga.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dcrtxewx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jfqzesgv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ktxhvzix.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mcfvqrmx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nkyvsmnw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3flwrulsp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3erpecejp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3qpxjqqsx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lldhjkxs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ufpsjaqi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3xxlfyhex.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aedwsiyh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dmekcooy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3gcuwdpjh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3fhakyqbd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ntoikpbb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cnuvggih.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zljunbkg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3pbyvmxut.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mkzsezui.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lcaymbqq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ukbftmgd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ufkhvixo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gtqjlsju.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bhrmscjd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3dwhsiivk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mnflmeri.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3uatozfik.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3kdhqlbhq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vqpfttpp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fraatfta.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qitwgvjy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3opvudcum.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hqdyxsth.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dfumipxz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zlficdus.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ziepzntq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rlezsnhg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3szywkbzl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vhonoefa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3poajhgwd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bgxrvzmo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3vbhamifc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lrgfoyyq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ufznwdzh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3iiycjpxb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3jiwqprhf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3nfcaawlh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wygpfkhu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3prblwusg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3shnbflds.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ahumeexm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3igazzapd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rwlxnfrv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fstbnbtt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ffslupiq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3uhhcobmb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dqlgwbgu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rgajjzxq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gsfcviit.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fuospdwc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hmkkfpwq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wtkhucyf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmqgbxqc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mnttsfxy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qekxrfle.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yydnimcm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cavmkwwo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yxatvkog.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3hmejhxho.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jhrnmgca.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3kjqudosd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cuaicllq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3srqmokba.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yyzmqexm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kxphallz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xbkqjiwg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xmpotkgw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mpxrejwx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rlznnchw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rfrpndrv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3qpshtyyt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3zqagroyx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tktrzjim.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3paofkejt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgfsepoo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ybdmcrdl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fgslkbmc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qzjfjsqy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3agteslgh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3amnydpql.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3bogcpmwr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zpxhyxtb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tehtasvt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rekbamfp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ybhdhpaj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ibvmkehy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cpilyyke.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3euqwnzrm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3giuiurwd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3fwmxlrez.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwvnlpgr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nolkbebe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dsicflod.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tuzdgsbm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ahownuyz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ujylomoy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3sbbgwfgd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3klmkhisc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3oxcbybtf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ocgivukg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqrrlyag.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pdrippml.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3syequztj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qmupizoi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vruczwnp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dpctcpmd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tjpitphe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gqfffiky.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pnxxcaqi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zuykehmq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ducvzpzx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ivuyevxl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lueukbtv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3plumxpxt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kyfyukga.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zqriapjh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nniozjtp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wfvarudz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ecdxrspc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kivmoctm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rfaqxhxh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3trktjdcc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vwfdunnl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3eaxfedrd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fqtluxwu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xxpgddoe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xptsdsxi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ipzwxvyj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nsagjxir.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xwsbsomb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3cfvgaqds.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nruoxkbb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3bjzdwkwt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hmnkplai.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ibmocqru.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nnkfeune.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3indmqvku.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3fydxvzqv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xeufnaej.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3syppeujz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3lwzwqyks.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3edwwswch.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fquhbgwh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3iujqjxly.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zyalaagi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jhndffpd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3prvtgcku.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3unyqxptm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ktohlaaj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rkcobxdl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3evnalclx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sisrwoha.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ddkerryf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jxkjueew.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pvhzpqzy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3axivihnj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bpjrhvwk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3muttxxix.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lqinefyh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jeyxuapr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wtealbuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3losdmhgv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xdwmvfcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnvgvcam.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lewindlo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qofpgnlo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cwefxuvy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yaabbiaf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3aswpxipg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3mysxkcno.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3kxgvtrnf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3smtgusga.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fojredmm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ekzcvqbi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3evruzdae.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3eueiqenq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gzanktqs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rcoyuozz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3afdazxqf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jkzrgike.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3izplulbt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xzanyzbt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mqbnlpup.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rwobsxpx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hlwlqtjn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kokcildh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mafbvjgh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cbhemijp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3frmpvrhe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3npyltdxm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yqnczvic.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jfnlumnm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3stackpva.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3wibpzrjm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3fgbudisq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uhffolxz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bgbtzgvu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3cwglsflj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qsbixhtx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vppguatd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3hdjmdvir.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mvswpjjk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vzirghbm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vvmtawzo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3naaacfnj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3arjjxdlg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3yxwqtxbo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uewcqaap.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mxadwwwb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mfvyjjwa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmcebrgn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tuxuixcd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hamukkql.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uovdbwzk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hywklwxu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ruzdwtds.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xlnfizdv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gvlqmxzs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ymsufysb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3fphrxowq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vykytzlt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3axusyeif.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ssjyhval.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lrlqalbx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3kaolgzsp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vkpdnmrm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jduhtjmx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wdmbnzxa.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gfsjipzc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ynjrblxu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bciohxsk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yszdhsce.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wjdiajhq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3emowobvx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ynzflecp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3chpltqup.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xrewqwug.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lyrrsrqb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cwbrdilk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ktsgmshp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iuaoqpkf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tbrrplmr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3rhxydtjo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zfdhlcxm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vinogpwm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wkwzurzs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3blrvinoj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3lvgiwwzv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fnrgyqqp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uqlcdazo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3watlanla.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lrehsctt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jameadke.html


<!-- 参考信息 -->