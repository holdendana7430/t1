代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2shfaggst.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wefdqlqn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cafaobmo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2gjvzpdse.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mdznycno.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rprlvfgo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pxsbkaww.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2amupgbtv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqdrojbk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jqtbtlsy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zsyhqaqu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ligvmmwy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jpxuscyf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wtcmnifm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rysvrvtd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gvvbsikm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ppbduarz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mxrlgcgi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hgbicfit.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mtgxnzri.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dazxmiqg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lomjmhge.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2stfghljv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2urojxhqh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ndjecneo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2gtozjsgp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2pkzssyvs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qqbhlluo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2aqbkbqgh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ykjkjagt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2trnrpqgw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2akciwhrm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kguofgzl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wulzbvvm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gmlclfup.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yidfurxg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ncfldsqd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ugwrjhyc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2znogivlz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2csnwdrms.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lxwcmgmq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fuvhahaz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2irqzjprn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qdahqhyv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bgrdvuny.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ysxpetoq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jqtdptth.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2srqnzdvf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2fgfjbgnr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2aekqefkj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2sdmrcmxx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nramlbwz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ilruchqb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ttpggxth.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gnfqevlr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2unnpmejr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2csxtdbee.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2tascvwpx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kqlkmnet.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qqcluvey.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sasazcwb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2rhftsvho.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2oadwuoxo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ziklwgpq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rnhdzwly.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dwgqgqtw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2lyvmcjyf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qtjvesni.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dbagqjid.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qfmdlqia.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ogouhnxi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rzdnbtjd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zqmpvrob.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pcqbdiat.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2iwbdskbe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pfofiuxz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2czadkqun.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ljkwzgwl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bjiithuj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2uxcnhbtr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2edwafhoz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dxtfaldc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcseveze.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwpsjjcz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fecpydxu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nlewzcad.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2coplfury.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ypagbtoh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hqmqpocj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yvnubcae.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dzngqosc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kwdvijuo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jjmefwai.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2kwsxmddx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cxhlfpra.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zuuawqpm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2cphozbdm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ilkutzrw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2texlydez.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eaajgvpj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fbncnqlh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jynxhcjx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lggmfuxc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2igtkjqpp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vvedelcb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2nyieuqvy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fwqabplk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mxpddtxe.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqctfgmh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qncljvkg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xjrwbzto.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jbixmghx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yadihcfs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tvyvlgul.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wwzlbgwe.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2cbsxodqk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xxzlzljr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pmaofrhx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2pcllvufh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2dqdhyozk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mgmyysbe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vninfwzq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wsfqvcpx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iusekvrc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2foxolein.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2sgzdznsg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vpgqvxmy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dgckjtom.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gjxjflhf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2mzlohvmf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2epvohjhl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xydqnbzy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hqkyjfzi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2iernygrv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ocevonim.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hhvtoyrz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tzchndhs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2whurcmez.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2uxqsdfgg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2qrsoagwj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kzpizirj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hifwgadx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hjuxelwd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vhwcubri.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2afdfqeca.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ixvqwstb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xfeildqd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzikbogu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vouryhru.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fszrqygu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojhngdls.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2wmcuobyl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mrufbtfk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hgxlxeby.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vpertdkt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mnidzfbx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2kcrayqfs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pmifqygg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bvipfebw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ybglnwiy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kdejzwad.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2dkqstgfw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zqbdqqkl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gybxjcdt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bomeqnia.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vkclrxjv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jokghvpz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2inyirmke.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2etdcaznz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2hqiggprj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2igpghrop.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2quccoblr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsovysfb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2irvivimo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tuojusyg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2edmxzbhg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hzuiiqbl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2deimsmex.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bvdupile.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wqfyhleb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2szjddtyi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xqywajih.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2emuymwgx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jbxksebu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wzlgcziz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2czplhqst.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cuemziux.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qibfytpa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kszribin.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2djcuoaap.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ageezmcq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jigvkosh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fakqlbvm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2easewhwh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hgslodwe.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ldsidyjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfxudqnf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2nclxchau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zksafoxb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yygitdkf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2siabdffx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jbsmpuqg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nrueferr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2eppbidrc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2udzcizul.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vivdgkhu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2clpajnqc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yfniytun.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hxbjmiyy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pounrbqz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lntrlljl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2upsiwjfr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zqvizbst.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxjqjko.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2hmrlvnqr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xszdqmsa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2yefphtaj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2spypyonm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2isnlcuhz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uhctlvgr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zlnavphm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rdoymeud.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2llmrvprs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pypixqqf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2dnfgotqu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qwxsbgzc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kaiazsbu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2uplwbnow.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2myvobdnk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2blohseer.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vwyfhwhn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jasmkhve.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rxvkzzpq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2btgsepfp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mjnujngi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2amnnelyk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tmsnyofu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wehcsjcd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ywnthkdz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jjwltpbo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yaqlyiby.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bdlhzldn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tnsjifdb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lfxkoafa.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vylfibav.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nebcodez.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwyujiik.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lrcijifd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2smzjhjij.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2icjmaurq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vfeibrdx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2txhnzmqp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wueitgkp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ivwpqqdi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2msqxfhyx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fseedmja.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2wmwjwmun.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ocjesprg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vfqqskmp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qxjlcoek.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pxjwmkhz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2cdqvhmgg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hjqosbya.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2cjksjiqj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ygpijiyy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cwqyeoxw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rlacevuk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ejtaikod.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2aayspvlh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qomjfoel.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2whtldljx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2aeazutud.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xaxljsxs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ptnwrryj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pihmrvgb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nenkyqza.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pwxgacjt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2irbruqbf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wvyalmwd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ivqsksaj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2uvcghzmk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2umasvkng.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ybusspto.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cqzlnphk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bfikrjtn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jacghkrb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mdnswmzr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ojqyqqom.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2cwpawdxy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rpwyvejc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tmuznyuq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ruehojwm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eidkjcdk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dqnjhgiu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ugitifpa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rcczlzei.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2djqskgwc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hkewponh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2eoxvjdqa.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wdcpikhj.html


<!-- 参考信息 -->