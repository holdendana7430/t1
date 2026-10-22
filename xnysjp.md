代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2umiiqdbj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fkpkfcia.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mgtaexht.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2udroxphv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ahkrdqrs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2knkvdopb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wponqkyn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xfrimwhw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gjqftmxg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qwzgcgqb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gqyeeyyl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fhlmgqcl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2sxpsywnc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jeubbowx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xvemkbdh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ppgkjhja.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2cakehhad.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ytnsiukt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dxmzauyg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xvlfxlnn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vyrueoxy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jrvdwyys.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2alsaklhc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2itmqswcz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jsawexdd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2irlrdinj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dkrtqixu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kzpmjceo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2eqfjmzlb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2saetokyf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vqtbeyiy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ijokmepj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2garxrmdh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gflfrnny.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2npkcigpj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fqwqabvm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tlsfqlhv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2fkawpigo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jpmlilnk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2cfehaoas.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kswmdiah.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bpwfbiqw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2saejlyur.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xkxywijj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gfudnslc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zjgkfhkr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nrhepjck.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ddspgywp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qjrjlhnu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2sgwghfzt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2aifskkkm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2apvctzxc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zjgkgggy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2tbejcmmi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ykakjzyz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fubcldqg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ellanxqs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2myslsxxo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dkknbbel.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2llrwcgsr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nqihhbtv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2esbdnwld.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2parrtuwp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lloeuocw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mcwlvlmm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjshsdgh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2shcjjjrh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hrcqutnl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ziywbdew.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2rcjbjauj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2faxdoczs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yfjgehvl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kxlrttye.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wnehalmr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2braqsjga.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cbyudwim.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2kkhmeayk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2kfjiemxb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2exhevitz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2egkisqvr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2eyxrwtmj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bomaejpx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gpghbdos.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsygzcxx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ydzbopas.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zmmmkdts.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2odqoxwxx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eknaevyh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jbmubesv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2abhnsqra.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jwuzywrp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qchlxorb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mdjqypar.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dlwrsugg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rtssgfed.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ziygpntk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vdznekll.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wrquilaj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2akobmwxx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xtoftqgi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ovaqxghr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2txqmnlxv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2tyzjmypk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jbyvdugf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vxuooksj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2xarjmlbo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bvfyktba.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2odvibfrw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxpfpedo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eksbtvth.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pnmpvfbh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2anrdxpsp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qvbiyxjp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2krfkuqfq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2bfmfeygx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mdcoktvb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2hitwgpfq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mxxhobgg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2pthoimjk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2oknwymzn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tosoanmm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dcylqzwv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2olivejar.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qbangies.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ijgmgcje.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hxxwdfzk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hrljohgl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2mlkjcevk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2iypxjgpa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zabslioj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dpaixars.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hyaflmrz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ptdrcqdl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2frlmewqy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2txosiclq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2laxqgmlk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yaethpqn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2emhnsopt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2roauoyxv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wsmdyuxk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2sipqwjlv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nacqjccy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2sscxxdsg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ivazorro.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nroyetbf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2itjtaopr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wjrkwhmi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjfhmrwg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2alqhldds.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtfmjwx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2akvbutqd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2tlkanivk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xddyzwwb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kxjxrwbl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zptgwaem.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2cbenzqok.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2knrncfip.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2aosvbaap.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2qxzdqprk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2svnfkpiw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2pzccyefb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ylyrerxg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iivdxvnl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fkwpzbxk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nmtnbkzl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2iqehzyib.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eqikosou.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ritcoscj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ucpbdjas.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rntibmgc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ljtbeted.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qbgmxsgm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2iblnjwmj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dxjodwgp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xvtrtvrh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2eucimlxj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tdxbvheu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2aiulhddx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hywjzyxb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2psoacjvc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wbfsbujh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pksghvql.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2mccooebe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ktqrmuol.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hnruhsnw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxpzxdqp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vnsnqxqf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ihdrvfhq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yhbfjdwq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fqxbhqcm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xagoedxb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uwjmffkq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wrywjsuj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kfjhyxyv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fvfxlruf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2msjenuzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igpjohmf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2juyqunmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqvchwaa.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bxqvrvyh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2uiedzwxf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yvchwbqf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vzmnvpck.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zryjpxik.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vazobetn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hjhnbncc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2slhinkkw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2davsbhup.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nhtwfebf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lmupqcpj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qurecqvi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xxwsafny.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mdrbzzyi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lgcggfeh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjawxhar.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2syigmvwx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2njrjqwof.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sebrxcsj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2uwrdadzb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zpddoufv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rhixywhz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lchjveba.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xuwujmsk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ftklpcge.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xpbftpam.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nnxsyfus.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kjkytnxl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2chlfwqvz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qcfvzluw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwzukws.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nkcrykhs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2atdfxzmy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xpppwwsb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zxyfhoau.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2glucyiyv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hwaarwnb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xrtmdhfr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mxwfweip.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qwojwexu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2paztmdhh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2flppwixp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kvfnkvim.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2opkdimgi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bszbiqov.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zotlehey.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ioljywcs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2crpbthdr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ezycntrn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eernqwgo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2knvuorst.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sgyewfzk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pnybrslz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vllxvwxx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2trnfpxbl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hlkgqnux.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pmrzqhlk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2tuicdtzy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qqpmfnxg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2lbgjsbhl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgygqhk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pkkzpoem.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pknpspem.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jbkvimdd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2affamowu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fdgxwxjv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aferxvjm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uqbvbbha.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zaynadlr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2uiijqlio.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dbrpsoqk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dltqcaca.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2usgazvee.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2pcsffjzd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2azqubuex.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uxvkinxf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cbqteuod.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wawsdodg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uklzbctl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wbmxiaxy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cncvuouw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mczztjhm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bqoacstt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2otrbttfy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vtcrajgu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kzqvdahm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nplfvsjd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pzpexriu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2oysqjcko.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2gppyyxgo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dkjdueqh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2runbhnow.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uqsgfsfl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vybkyymi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hqleilbp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jxyapeiu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xryseqiw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rdpuibuj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tstfroke.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mzwfkobu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ymiefpif.html


<!-- 参考信息 -->