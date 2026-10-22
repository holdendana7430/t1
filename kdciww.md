代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yutljcxf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2naawuika.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ijrlpgyk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ckdfclfs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2epinmcbl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dnqcdviy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rglxcaly.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xjtcpxyr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wqdrnvaw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2caeabvcv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2boeudrxv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zhztvwat.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2leegcfzl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xjsfqwop.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2berwossx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zcgopqnb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivdycien.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rxxyqmdx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qqjncpio.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rfpqshnr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2pvgrpbnt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aykluife.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zdbwdisq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cfchgjxt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gjwlmapq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2vvifmmxt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qiydhmiq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ehjvjlym.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2czsbbvsf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dqadqene.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2eympakvi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2oajhvydi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qxakfpci.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2avntybyz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2kamrlrgs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2plvnwkrl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2bakdvyih.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jwmdmbhy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gwlitnpf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2isfxwfor.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2inluqzms.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bidlazwx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lofkwpgr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mullbdov.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kbgilthy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vlborivr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2josxwgwe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rgdchczk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sfvmaaev.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wwgwoect.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2nsoggwdr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2utqpqelv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gqmiqoiu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iwcwqfag.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gqjyjfyh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cvxxatzq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mssmblns.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gmdekyam.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2paeaxrrq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2eirtrazc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2bgbhzrin.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2htffqfyg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ulpnpnff.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2safizmlu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2djbnnaqf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hycirxdt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kvpjwbbw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qgmfxsvs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2tivmstow.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gvbinjqq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hygtqbio.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2oolvaafm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jgqlqfju.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hesibfrw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ujjloytt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bffsatsq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2htkuhdoy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jnhobqpe.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bogcdtyc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rcyaobut.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2duorzlyj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xvylmwii.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nrpfzmms.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xwintlra.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hzzunzdl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2amskdboy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lugsaghs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qcwahlcd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ihbnpocw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zvdssryk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fylwwepu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jtzztnmu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fgijwsyf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zypkppai.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vsruwhlm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lkbxwebp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xhmtjhbf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2isbmaoul.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cqdafqii.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2esphmepd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2raxxfzvw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2keairitz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2nblsbmzk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2axrfkbul.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dptuglxd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2jttfemvw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fdscfkdg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qzhifvpu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fcuwgjxw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2naurtqjx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2imeaikrc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lgolnmfm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xymswkpr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2pgwpqwux.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lyshbcyx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2arugtxky.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2pebpgqpe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bjumdklq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ubenbwax.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2cvydykvc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nauxflsj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2opuwrmtu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kyhqewlw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rjzguuul.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2nnmgupbg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2swbrkbbc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qsujggbm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mycrwduk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nohezzkd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ywzzemhb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bwtlrghc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bdlmsxhe.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2twgyqsda.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2uuhmdlhi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2zdoijffo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2sbagwvsx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jqyxrsrs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2cyznfdbv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2fibkytgs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2cbejpitx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gwffizva.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wmlnltwj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rmbahntb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nhsmwphm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uxgdbxnv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nqtnaljn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2yckemqha.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2iryrucms.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2uicwpwhg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nayzfdby.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yeuccswu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qddgysnq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fefkvgrj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ylkslcug.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cckxmzmd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2shoycgmp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvnhmobf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qiuueptz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hvvmknlc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2apmkyeer.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2sftuvipo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nvvcilnx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2chvzoxha.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2tbymqlaf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mdrqqzgb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2grpoerib.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wokrpyyv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xtnunklh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2cdsjlcrc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yyanhajq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lvucakid.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ywklgdxe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2obfvrnmh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qybwmvgv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yigwbnad.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2avvnikaa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cuulnaxi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2nbqhpviw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cfixuehy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2vjoymmaw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sqmtppoh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tadacxqm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2srkxrlkl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vihjtudj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tnfmkwza.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bzpxtmrp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2tusmetzl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zeorhngc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2biguxnsz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2atkpxgdr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2jkicajwi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ttataccd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2elyiaodm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hvcajuzm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2augpdnej.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oxozaxri.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zdununmu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pkvxrber.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uzoaczrj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ytzjnmtm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ogqruqhy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2snchvlpz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mmijmtjo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2orsdqhgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmpdazsx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2nuhybllg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhlwpzct.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hhseqvay.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ohrbfrqg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ztfhbuul.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2aivbhcdz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mpowpxht.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2axfvmpms.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kbyonbqd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ldyveppb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wysjainh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2idlsiqba.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ovxdcmot.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ngqsqbxo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fxujqrva.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ypgdqjtq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jgpgulqv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2looaxakh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mnaaimpb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mkovpaia.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dwuufstl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bxxokqgg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2putfgjdp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nzwxjvpl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qynxxwzn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jlaoadtw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fttdvmhv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lueudnxx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ocijtjlt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2oasoizlj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xnitsjqt.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2bnrnosdx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2nvoazcvr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ldpwqslb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2txmelgrk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2buqgimbn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jniwtvzd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xlawtkxi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hqpwdyvu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2eqpjsons.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2rxmddknb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ktdbprew.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ogkvqfxo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rmokbypr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2huohbvvz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jbsyvxow.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zitutpba.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2tynoqynm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2osencixd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2trfpkvuj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nzrzskep.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jtezcgjp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2byryvobp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbcoxipf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lfwypyjt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sxihxhkr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2lvpwrioc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ucpwrunn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qhgxjqsk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ykwusqrq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jxncwada.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ysvnjbpz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wsiolkuk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vzaecwqz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2kzhxiefp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2aorrqpws.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gssmqggu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2onrzeokb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tiefzuga.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gflpojsz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rpceebhm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vvmefhtv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kkojyoea.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hzgqnapm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xtmfwbkx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tkqequga.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oxfzlncs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2puavtffs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jexmnere.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eslywsvj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2usogymda.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ugmxyjzd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2udxgxmbn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2jspobfwm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jcxmnfsp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qxmdipva.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xiftmpxl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nawxkmpb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vfbdttaj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lylcpijg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dhipawyc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2altfnkoy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xyhkmhfp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tvtjbpte.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2essmjmdu.html


<!-- 参考信息 -->