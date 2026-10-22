代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kevbbqvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyyqvjjo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wpqpxbht.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2llkoxniy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zylkjcfn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2thqcpanq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xilbpmyi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dmqxluav.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zgbrwlyf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2pbrnddci.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dauwwswd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xlmdblyb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qkhwclkx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2znfcudaq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xwihkmxa.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jkgyqrjm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zwqueqok.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2czxctsec.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2oymvjggn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fdluiodf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tpfwqdqv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2liofnidc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2zuxyjjie.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2alkslouw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ookrwmac.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eqoromvt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kdngfhpb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qcwbngjo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dweyqbuo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zeitkrvv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2gamgeqej.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2osnxtugq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yjvqcmvf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2axrdjrtr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2vcnklecr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mxvdsqcl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cszxzirp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dofliepp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2pwdjbbvz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kkfsumop.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2erntaygx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xmszlcbu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2bollkjhl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ezdbllev.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vivurptv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bbkdttky.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mdyrimiu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kinvfcjy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ntbupmaf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zaqjlmmv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rqnkyplv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dflqapsa.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2frquocwr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sdmuenol.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2okkbfsll.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2sxjguqjn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pfdsdkef.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2otghfckn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2esdwwhmf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qbjfskws.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2llvhkakn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jbulsmkg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cuwfsefb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dgoqxqxg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2oqvpftjw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zqtnxoaz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zhnpakkq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2yzouealu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2donjpcac.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xphwpwuv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oydfcikz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtqifhd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2hqwryciz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kqevmuil.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2wgdrcotq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bcpjifhr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wuecmtgl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qykwbyqe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gvpiuyrn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2umzhdtlj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vxukoshu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dlrhpegz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cqveqoxt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2elblykou.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2yvwdgwqf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sxhjutwp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hkwmkcai.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vdqaoykd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2lgolrbwd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jnadwdmc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xqpcrinx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2eweuyusz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rijmtbfe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lnyckbbq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2havrlttt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wgsvkaox.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fbjxjjqi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2dpfwzsib.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2yudzcutp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2mcbqzfye.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ewaplvsj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2rsxcrfyk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pcgkjqqy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rwtqkxfr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sjhtsfvk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xpltqqic.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qvcqojvd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gwipqvwr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wtowuhkf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2gezvsefd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tfexiesv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rmzwjvcf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vsgqjfcf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xvswhmqq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gujgiofs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ckaqojxo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lpurzbdt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2shtssnuy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mbxhdjha.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2udhfsytp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2szyrwgyw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wxwsjocx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zmuciasf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndtzohht.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aftxmlqo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2aqngmorl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cehmnlmw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2epnjiblp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2aovgkcbc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mygqvhfj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2rctflice.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ippqwfzg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pvuzazcy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zytlvfck.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2knclpuxv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xgogjasb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gbmiqsep.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ybixrbgb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xwwjufdq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pchibrez.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yzokmldb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qygsisho.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ayzxlwcb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2rpybhwaj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2evkandpj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2veytcuof.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gcoegkxu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2giczejme.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wmxpijcm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2acteuqvz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gfljfvbi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wragejcr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2soyanhrr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2eftksaez.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jascfqjm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tafhgkkx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ehbhvcjd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yioyccgd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2njopxpxs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vzygbnnk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bqdmivsn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mpidnfcl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jexisgll.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dsdauhxp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yenejlmv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjzhthlr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ndzabyvr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dbayteur.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fnctqulc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2byrmbyea.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2baftsdlc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bzmrzjtc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xvhsvwyo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ixlzifeu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2siskxnro.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2yibjgoev.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2swxtxwkr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sdnueqjm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2sywggkfe.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nkdissjc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2yjemreli.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vgaygmam.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2afquqnbg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2djnqmbrs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2stixmfpu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wlzbowpo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2urzlkyry.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2quzfenaw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qbcfmaye.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjmkqhkq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cppxanhk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2pouatjjq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lafqpixu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rcpesnic.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2epxnjiuh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2isrjnkfi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dumwsjxk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jhsjmphf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2swdhehkh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jqwgbuef.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mmeuecjx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fdepvpob.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yrgdzgfu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2slcjvpjc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tqwpfzpb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2scszxuvh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nynlcqfl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2lphnrucb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vudhbtdf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2tjfpzzep.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2eytjaudv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gusqxziu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgkkcqws.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tfayudgz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2sjjqzrxw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2eurooueb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rqaoreuq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tzhrvjkv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2iisguczw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2flytbjnk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qdyayjyi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rmezsjbo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qhbxxluy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wmwdrciy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mjddcyvh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hrkjkcjb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2miuuiyrm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntwbpylu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2cyzuxaqh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lbceoklj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ujrgiurm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ewygyird.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fviahuwn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2drnrtibq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vldtying.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2slhzviku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbsdoqtb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pckrabqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hndsirao.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mdsinjsg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2igqtduyw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2nlbugabb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nkomztwy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qkwapmca.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jgbuyneo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jfxtgrzi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wuhedubj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uxgohamy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2srbrjufu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gsavrhqw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2augdtaqq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ivllbrhl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ekslilpr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yfbolasu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2biggdnat.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bwwefzzy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2twurxpsr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rrbtnywy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2hitmybut.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gvdrdnnr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bhyzxurn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vgkegdsd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mlablztq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2srunutxp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2hjcmsova.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mytffpha.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fmwcktdc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ipteetrn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2stnmdnow.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhhkuels.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uepyaugg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cfxsdbkz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2lwakuvey.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rxkxmfek.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rcxltagb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2eadkjqco.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ctcaowzv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gyfkwesd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qzhapwnf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dxlebncr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gbetifpp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2dqtsbkdh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cmyazyjw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bnnqpaoy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2trqgccbo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dnvbkgmn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vwdaqqqb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hnbtjwaa.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ruwunaqu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rldxjvny.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zfnlawud.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ozbuebbq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wfmgoqex.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tigitukz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2harweouw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nfwnknmz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2aslhlpzt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rujbalmi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zlqnvgxg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xgqiutos.html


<!-- 参考信息 -->