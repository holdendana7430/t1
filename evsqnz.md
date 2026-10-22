代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bzkibmbb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vdrdcbcr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rmcrfbrx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fhlkjdtr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vchzcbdf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jfcxyliu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jzfzogrf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zyfibfgl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2dqttcybz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2irlhcddp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2yihlvfao.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nsshvhjl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gybrbuju.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2quhzfitl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ayfnpncr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zvcoyyvh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nzvcufll.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rsjfnxui.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fjogqlme.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jorqulne.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jufhyctm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2skarqrak.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nifyjolw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rwrziggt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2cgvwuxpp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2casrgbxg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ddvhzwdo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2eozbrhfo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cpwxybut.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tcrhiswc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2klmmxgyl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ohfyqknu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qnoxcgea.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cqcbgcks.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gmytstcq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ahcgtzai.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rydtqxqb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kbmepgdl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2pwojupak.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2cviqhpvk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vycnbren.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ctzhxrvg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jjzawztl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2eqblullt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2dlpsrlzy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pptpovbb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ecacjync.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2otjsffks.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hrhijilm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ylenctuu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wnieqflp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qkcboftz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pjwlushe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ujuxjvjf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejwccrun.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qyiqmzsl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2byixspah.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2xpdvglbl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bhgyxikj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xsmiekar.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yrlaxzes.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dyhftyby.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vgdonotv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nrpvxpsh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvthdism.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bazdzrnx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jqctpuiu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yuneibdi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2dcajbxft.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fnunfcdr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vkiwifiz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vvalphng.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lzvqbftr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2fciwbvbz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cncmacme.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2fsdzjrpl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rhsimweb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tcqfwbxo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ndcwmxbm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hmwlafkf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vplqhhiw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ryvmpcds.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bknvnwja.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aqcjgsbz.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2aggklfvs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2whopzkek.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pwdlcvvf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bgjzxhhv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zegdgqxy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cfhougdu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jftxsfcn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ukcxfcom.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uomidoxt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2icefhhmn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bmvqmufi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2itnkgybj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2djglrizn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2muexuvpt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2hzylctwd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2veqksgbg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lyobqucz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ofhpudon.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jkfcxghi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bftaaewc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mbvvmmbn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mfbtarmg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2exqbtxcn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mslxnked.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uuofsqdd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bskrstqu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rstroohf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gkhjiqcw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jkzimmbs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rtgrwamv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hvvuhcim.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2aubflkhe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dxjybjoj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2oolyetnj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ekdomktk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jutjauef.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yxuemxtf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czlmctmk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yjxawxlj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tszxeyse.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zlnjtbvj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2kghgfpfg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gwyepyvw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hzcygzdu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2efaegewl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xqqnwoke.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xztclmvp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kxtynkmd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vjqkdyxx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fqvejbxw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2eqpgtysi.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2avqyshbp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ymbzztah.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wxhurejz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zgqqygsb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ayfokgok.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pzibpduu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlycdyqt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uquajvrs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vmvcfkli.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oibhzmdi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mqpeaxmy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bmenunad.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ivftjmsz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdewawzv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2eplxmjyx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ztdstxbw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2wnbcckti.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2agdvnyak.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gzocedgu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lvvfqefc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rknwllqp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2napaltmg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vswcelna.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lpudsbnq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bvvqvipm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2abcosmui.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hnxmfuxm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xddwrexd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2eclkxutx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2egnchtno.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2riqovpyz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2llzygokz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xvhrvawl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vozboltl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2grudmeyd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2qhmqhswj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vbhhuzbg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mpbevafc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2urrqvmwv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wgjdrxpp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wnuuhwgo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2diitloim.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2tphguwbf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2itnyovfg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oamfbcya.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bmvboero.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2usrctvaf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tntgnyxm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qvuqcxjp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wkrxvejj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vjupfepj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nljwogio.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wbcsffqo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nowjkpez.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2txosbmin.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fclqoxrt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vsjieofu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utepovao.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jbwxjdzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwdwtswm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jfwsobuf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pzqunnra.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xogylmql.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xohjbxbz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zaxvflck.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xdcqjfrz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2agwvjjcw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ieebwxqn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cwpaaqie.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2twssteyh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lqvqmuks.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wuiutuih.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2etmhmzvp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mgsvngyi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pykfllgt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mnkndrvs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rtvwowev.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2geelxdfl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vadurjgo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bhofmyrj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tlqcrxwp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yiwhhjlu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pcofuauk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cxgjtsfn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vqsepxzl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2moaumyah.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tywxwllq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2cbmiofpw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xnoyxugi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ejddlwip.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ngminjzy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vlzkeoue.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2asxlkqpf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2bzcktzqo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ryxbcdat.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tstzjjfd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2zkhclkdt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vkkxligm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ykfwjdfn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vilhlmok.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iagczvqy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oputxtze.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wqsscuef.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ftqpwdyg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2emlyjcoh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dxmiluue.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2apmoyavk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2agzdsbdm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eshbmavv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gotqfwvf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vdrczhzc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pgzqmaea.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nzzotomh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ezpbrpti.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pcqpkoea.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2awjeytrq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rijctfdf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vkewmvvg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lukhcycs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2kghcshlc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymkxdwfk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2okvglrlo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mirwwfun.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2walneygq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pvocdomy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ztcaspch.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gaqxijic.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xfnylsev.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bcxyzhow.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2rblbcdpl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gwfjwqku.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2elrvqjyv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2awwpqlar.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihdyyaoq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ldrsduoo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qqnodaip.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lisrgcfb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hwrnbqmp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ymncmrye.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fzkumwqo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fqgspalg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2huctjcaw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2krkyixij.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2shaajnoj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uwygneqv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2njipeodu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hpinxdqm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gornntry.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gdnmcmyg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xghlctxo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2imexayjp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2djoeipmp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nxteeybw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pogfpcte.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ucgvtrkd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uufjwimz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wzzlqlzj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2orneirbi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ydxzdvvy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qvarctet.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mxgogogg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bnryrhmz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2snaheyhq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cfzjmnoq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2usqdkban.html


<!-- 参考信息 -->