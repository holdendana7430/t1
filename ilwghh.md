代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dooxytln.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jrokkvxr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzlmuqy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rxgfpjbk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ptwalsyu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2pmthyurj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ueleaakb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dkbjvsxi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gjfifngt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2prdhbtjk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2emvlsuhj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hoirzuvw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2icpymkvs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qssfqndg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2dfvmajzj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2kwgsoazd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vsdjqnon.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hnjiwzof.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ojvpqlmx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2aiavdimr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tzqvjtfj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hepivqfu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hheydnff.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2agltworc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2autmdngh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fbuxabwx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2yhjdswgc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bhrvljqw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ouoaigfd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mddoegpa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zmmfxcal.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oghkfgrt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vyrvwcqs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kucjyeul.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tbemaozv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2agbkrnrd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2afwqxxkv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2otyycnwz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2sfdhsmez.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2weanttva.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2brbmcqat.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2njahruzn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ntqoxwuu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2zrlmxllm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2enzjtnwa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iiqsjsso.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2nvrvrmdf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hdndunqa.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhnhhqjx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2scqpcagq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dadqzkkp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kybpkqbh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ekjbuvxq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gwkjaytd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cpcwjnxi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pdymqxts.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rddvztqp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kqfipqfj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pbsitfdu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jhoikjvf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ekmgdler.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2sehqrpvy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hoxkmtqz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bpvpcrjd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2cnqktdkw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2luurzuxm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pgrbwbsl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2eoaatuqr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2cnmergkz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cobgoolj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmetlrcu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2majuygvn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nkxztstn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2nzmwnygm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jqpejzie.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jshmczrs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2eyyszywh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nbgeltzd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zfbttvhv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rjhgnzlk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ccygvlru.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2oiqoygvb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wrznpnhj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wrkvucbf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zmgphkjs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2azwcsctj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rqicgole.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2cbeqgbek.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ykxsqkef.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xmldcbiz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nfpmfhmh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wuomacku.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ewfgwbnr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nuktvhov.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bptwwnom.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2busmzemx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zfqalmxg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ncgnjamt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ilfzvmtc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wcxkcfth.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nfkfjrfy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tjbldujb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2vcdorjbl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hxtnqwga.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lgzsqdri.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2avoxigke.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qfhzdlrw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bhntzfpn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nndekyuu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gvdyvypv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vblbwone.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kxvkgtmu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uzkawwra.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2baitdzpz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2tgfccphp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dyzbfhcb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2wveuctby.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2chvmygip.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wdehorcm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oaekhmjx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gibyxpbz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2myhlmgzg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zjtthstn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2sitzcrwx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2powsezpe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xdsneawv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2kekgopqb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2legzgznu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xfdryqpp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2btvorhep.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2idebafob.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2yubyrvqw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mgawhqpf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yzooosuu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cuobmqjy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ebthrktz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2btlplokw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kgyzvkdc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vusptzgr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2kekqngjj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2epocolzt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2uewvyskx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2uclijlwy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ozwlmhxw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rweumxpd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2quxbpkhl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2yvppiflp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lsalglal.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tctgcxoa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nowhdvea.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gethacap.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2kqgrdbwa.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2xhdtklhw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vqhlqqnj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vivpimzq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2olkcpqqb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pemjvuci.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikmflxxm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wpewyxsi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bzsntdce.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2szkhtsfk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pxmmlcdj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2anndoyku.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2hxgdfeky.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twefuoki.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2suzobsoj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wftgjywt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qomexuam.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dzxlpdpq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2lxdstjeh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ppvloena.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vndmwxcj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wwiydgyz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jftiavkq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iwuiacql.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xbfveicw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yramxtjd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2uafjgeak.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2slgjslpb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jcgqruxe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hafvkyxq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2djoojhlq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ydtnmljc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2zrffarhi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2seekcann.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qknmuous.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ymwcvfgl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2fvqvkoop.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wxlhmlum.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wacvtcct.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cxticydx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rmftosle.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kzunlsro.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fwymwgfr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ntozgpeo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dawllgxi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2todipshd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2axufydmy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rxcarhpk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2fncjhytr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tfaxzxgy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ccnnzwao.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cvezzbwk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lpzzvarp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kydqaaaa.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jjdbqusk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jmwtvbuo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xjqvsdyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lytutrcr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tukjgayd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anlseory.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vezensml.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ewytqute.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2itoeccdx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tinmqfbg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2edfathjo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2dsraoiod.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vcbpqoym.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zocaratz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bzpkpnzj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rkxlrmtl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oeyavlhm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ozzajxyo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wzzekxni.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wrfqcemr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kulwlmfp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xjwyqlls.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mmffkjze.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dtjpryoj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2frzeisgb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2bbmhoolq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lvtjaqhc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fmmpmfik.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ruxcuuiz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2enrskjlv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vprkkrae.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tyskoufn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfcebnqr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2pzsivikt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tkvutecj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jpyzgqli.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vyalunsn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lkwwkeuy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tmhpkssh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2kknaabsx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rmgtmkgd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sjipxboc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pqgandob.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2pfpwwmsg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xxlxjhxv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ismiwogn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2afpdulpf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pbbywikn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2sylluuon.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2srqwslrv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vpivoimz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wnsrximg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojfqnvjy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uktccvkp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gjqbocyu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hmagqeqc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hmjcifcl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2otqkebvn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gcsslmmb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ylskxobn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2hcmvdpjx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lxzumhwr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gvxzdrrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2odthtvdj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xulkunxh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mogdpfgu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wgblhwll.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2sczhmckr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2pihhegda.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fubuuptr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ogvgavwk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tbuvfume.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nlfmjjgy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zyvwoied.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gqbiwqqi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xjkqbqhl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cdvknmaa.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sbqhxhhy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tgyyezze.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxymtjsu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jsxqgbmi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nvipgnex.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kzodmobu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2trwyplku.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lvpmvpfn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2enhdbktk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cnicmitg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ljynyvsl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pbmaiohg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2vtihpged.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nkrbcbxs.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2twbrpgzq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2msjgoxqt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zyiwhdcy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zqaymzjo.html


<!-- 参考信息 -->