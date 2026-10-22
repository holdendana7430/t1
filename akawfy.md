代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yifrbiel.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2warkniky.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qnxstnvc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qlechqdh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ymyqbcnq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gvldxfef.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2edtcamek.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hkmempqv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ibxxzoxd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ubufrxyq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ekiguvcx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nvmemuhg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2josczetn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2chgjsucn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jjxgdadf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ovbifoxs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ldzzlgav.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gfnxrrwc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pfywibug.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hkorvsmv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2frutmioe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mmdwabgg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mxcojjqa.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xatdopxk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2emqstcnk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tkgixyrv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mkkmggzu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dagzjrux.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uxnxsoin.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qwtombhq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qllfaxbu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2isncudke.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qdanrohq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ktsuiavq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2uijmofrj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vsuhnbso.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jjthdpnd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ddemvjas.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ghznulmb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2luupceop.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gqxjuikr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rmndqfzd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lzpqlulp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2apyeeeop.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gejjjvjx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2puzzsqwk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yqultiaf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qsildmdk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2juyzwsgr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2lhgerxfz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ulptldbd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2iauueztv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zhdivchu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qfpxoocd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tdssghha.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xkeuedxy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xkqthnuy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pgjjbomc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uhhgzhbt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dhletjak.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ylvrxqjr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mlmfmxzd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2gwraajsj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xceayzts.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gkepdepn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2iuzfyppe.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2syylmbez.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mstmapmr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ugdmwguw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2dkvtiodu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wadyivaw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jxltznlq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vtvfgdmr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2smjmlqwn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mkfwocuq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lvcfgsfb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xfwyslwb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pjgijsuu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qfcpjgst.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2clxgizuo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmlgpnzl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ntrpvsyz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2exbdmlus.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uqwextzu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bknyvyub.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pgfanaen.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2injutaqh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qbibrjou.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ygyuzuzl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2mjixyacn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ebxwolia.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vejgdwrs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rtljqide.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zggvsnpq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tgqrivnf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lnaljnbz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2crtohobr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2txxzknlm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pekgrmch.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2slqabsoe.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zhgxrdoi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vwfzmabv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jrwewtln.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2veduqwcw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fleripdb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2olkukepx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2oivstgvg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ukcuhxnm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hzjqzzms.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2fbwnztcn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wsidsvns.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2toywkdhc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lwfxonoj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hhlajcqz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xalnvpnu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2yelqlhcb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uuvgaajp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2efzhshwp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ghenaxme.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eajlbxkp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mazyrppo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xwozteqi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gflppanq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2lfhqmkks.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rthqxfjq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zqwrqrxg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cuhknfxq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mqepfvdv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tykezmnr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2nnmerxxq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2owouirjy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2eyhnlpxb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nuknkxlz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xfhumwxy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2worejgou.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2adqutzci.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zsioajyp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vueqlcdc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2tdaoczoy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pkpqphnx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2eltwuxgh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xkkdhoxf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2itnrvofd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kustnhsb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mfzixwzc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2rszfmlgw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdahaorq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ylznzbcl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kvzzpvwz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2oispgvav.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hzvgeawv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gufvyvtt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2sodfcfgs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2iswgbnqy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tdijaprj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ugahueee.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mucphyfn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2blpbhwmv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iebkycdp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ryegfmgi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tgosmkus.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2teqpwnyh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfrjvnjz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2trqmcwex.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qkxlqyqn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xburrtvi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2znkepxxd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2snvqkijg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ohgdkrrv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2buhfedja.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2yfrdjzrp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xhbycwmh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2yoxzfiag.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sfarqosh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ulvqcvwk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yqjycgbz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2axgnyuev.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rwjweser.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ynpgufcl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2phfkoggc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2mogiieua.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2styudxjp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2brrifefe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ihmkezoi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tbyumszx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ibunwqcd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2yvyekmum.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2sanyeyri.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hnmmmgri.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2btzcgois.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nnwwwxgl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2htshakhp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zveggbbf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iatblftw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2isntdzog.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hldjgxfv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2dmneqpri.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2efkfwgqu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dlrmwtbp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vblkqcqy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2btuyfycs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rjxuzdyv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kzwnqrwu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fsvwjqnj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sudfbsed.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2icjajlrh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fpqrekla.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rdxermbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkxiifyz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2eabwhxvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2toagtiby.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2egfywnmp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2cdvdgrzc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rnrdqsah.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jwqolkeo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pgswpsen.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rptyncsx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ezvtxwyo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qpgoyjsb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bmtuviwf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2nfobcpnl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mjyvwius.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wlqypusu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2adcrdjbo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fwsdirpp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2djojkfuf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ammqfxlu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2noyswyil.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2gzbodkje.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2invmvxpu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dpvvghlu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pejrtvnc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hpfsfzlf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2unawchwv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wmdpboyh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hiqzwkdh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pzumklei.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2viswulwu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2aerfbxoe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2frwponmf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vxwltnqb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2pvdcodyf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fogtgeqe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2njupmfno.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dcwriidi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2inhsywue.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ivpmqppj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2odeavkoj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2nxgvvygw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wvhygzvq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xmhiwfmh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wmvpwxfq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vemmtjdq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2foeolwdo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ruxqtifq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bhyrlfyq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2uflaajri.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dtvromej.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2alsisdhl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2isnkhklh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fyakgvuj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fwujiikv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nctsvsvv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2grrfcypp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yepnmjks.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bjgnjooe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zolbpilr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bguqqhtg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2znocnsxo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2esonsnct.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ptdosklb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ykebyphz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vsoppwgc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yhynfwga.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vmbvwhwa.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2obbnzfyf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2knwnpyth.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ckyzbedw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2klusweat.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tkmnmzgb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ihqzfyqo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uktmkjdb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2noznzbbe.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qczrdukj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gjtselzu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ztaoojcb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2chgyhfyi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zjracybl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ifrhfryc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2pgigxlds.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xfclqnja.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vlkjqoma.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bhrnosso.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fiqjtclo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mftrvhpl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2stnpshpu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sturuvlf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xszjuttg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qkeyyfrk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2byvthgtf.html


<!-- 参考信息 -->