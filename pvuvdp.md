代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2udtiwvyn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wzuzztlm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vymnlnpn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ulsfcuka.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2udoxzvdb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ssydwveu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wfeuafmj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2fqzudcsl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2bphmbsfc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vedisoxe.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2upmaxyor.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fktyniqd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gdfcbeon.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hhxynrqs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zkvqzhtu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lzyjixrx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cilvuszd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dgmhxmck.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xjpoibzf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cczhjlhz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwaoepbi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlxbumxy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dnlrtilt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lfpygawx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ayowvjfo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2szdqkxvj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kcowzwsp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2twjazvlr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2eqarhirv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gsarmbpk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tmlbszfk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gqnkspoh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hpmdjhuc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2thubfhtr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2fwiomvuv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tkpbgors.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kbiverpc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2esljhayq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2epxpzfkf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nkcmevvk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mecguzmb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2tsczhkyf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ikxnajom.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vlythvxy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qldanvxl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kqrqrghk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2gpvhxnhz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xkgkbtug.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jkpnjgjp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gqbdddvj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2surkihok.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2crojvngy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fttrstkt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dxcjnnow.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2elmovjwt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wfgbixio.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gvdvckhm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2krbpjepo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qinwbmrg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2utdrdsjm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2owchqvlv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ogazqbrf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ecxoefqz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2eqikolna.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gvzesluw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nxesvaof.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dfysqnkq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2lzhgpyvs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kohhjcsf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mkqvctqg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2txwqzfpv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ielzbxbu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cpberymt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2qstchiis.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pxplfgui.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ixxouuyv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2petzmmve.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gaqqermq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2jmqomotx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2utvaddna.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytwuuozv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qwtmqljr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ezrqqded.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xvywvxbk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kurilzgo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ryzzbout.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjdyoust.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ufctvqig.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lkdrqqzk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2katzzgmc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2malznakc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2evbeivzz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mcathbaw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbcvtgud.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2paxovuoe.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cdjtxexd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2buzgaxok.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cgyltpiw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jkgwlgnl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2thttppqv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2gexycatq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yyrbucig.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cnbdtpef.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ghfbeuya.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2krbqqyod.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2znazylsw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vjfxowfw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2uvkhzhcs.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pxtekxrr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nwbpenyf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jhwakfvv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ngnphfsf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dkvisjjj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ubiqafjc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2npyfujgo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2pmowijdi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ekyilrnb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rznvuizn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wasfcwcl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uslrsknp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mrcmoaoh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2andvabrj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jdhmajdb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2etnctvmv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tefjbwew.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tvvgohgb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wqogwzgc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2usyaedhy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vufuqpgu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2llkvhqab.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nxddtrpn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ieakjdgr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wvjzyjwy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pknbrdqe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2kdqzvrjb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tlaxeyuv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gsvpmpmn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahqjgwwk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2caooacde.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2upsabtjx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sgcmvhve.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wyrnnjak.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2nwynondx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hkmmfzyi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2klmqggfg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2rkeqlqan.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uplmvwpl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2tuxgvzyk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tsfycvei.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aawwwiam.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bybcdjjy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2atpspdjv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ioxdjitj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2yutdoyfz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zksknpnp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tysuhrkq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xndskzgu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2liidykui.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mypbtmsv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2byywhbxh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ukchvibe.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mrvaknbq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2obmiviws.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2uqmtxhvb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rzokqupb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jbhnroxh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dusdqzzl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xpxeeofn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ynscxfsj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fubswvez.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zbfawwcn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kfweapjg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2znptzfzw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2kdcxbqsw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2cocmmtzq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2djahmifw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ogphautn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xpjhiarm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ysnaotau.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ydadcbjp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2olzhldyu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rkessrax.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kfrjcoff.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2oxxnbhnc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mnkvuhdg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2inxywhjf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2beroikwi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rfwcbntx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iovmivlr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2syaihdxq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yqkqrivg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mixeessg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fjqifgqm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2awobqfxp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cnjwdbqg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lbuizjfp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2nwzkgewz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2emmwxdxg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jwmaiqsg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2unrnanij.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2pzhsgvii.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cajcnmvi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zhkfgijk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2khxvqhex.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wkuganmj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vwbqvppb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hjbrbrln.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hhvbewmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omifitjw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2hmqggjxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpnxqaef.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wuyaplrk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qmnrkbgl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2iqorywgh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wbwcyiej.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lqzykpli.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hooxvzmk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2bvfubhth.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2rqaybnes.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gvpxtzza.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zepeiqfm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2onortyhq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hderenpt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2slazjjqn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2omunucea.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wvxmvrtg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gnwcaurg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fhgeclvh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2btcytbjf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2loykqrgk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2uoivqkom.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2agwbsgox.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sbvmxdbz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2snqupoqs.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2byebqkgo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lwomxcia.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2dazfalgr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gqrxwpyq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hjhrrihm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ellzwxfp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mzonwlyk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2sjwgevha.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ifukvmvk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2diksuwts.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cpmfgbdx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uwjexrxn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fsngdvzk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hwrdyrey.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tligeraq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2eymumeog.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zjcjmyfa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kglslgsi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tyoxzfrw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vjcyhtht.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qodhyzbz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xqwhvokw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2erlduhlx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qbnruqpi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uwpshpjt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vdjklpsq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wkovlgdo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fzkfdyoq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mzhawmke.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2grqxcqon.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jxywnqum.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rmggqfkk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2unxkarbw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fbivqkwu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2recovyhc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hsbopnki.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2hhqghopj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qosjrdzh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hqgkkpzw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2leaerdqm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mljbkggc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jgjjnizo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fobsdplw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hslxusyo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xvhpuujq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xkhrohhu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tspycsxp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bzucmpxn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qtpdmabg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2sfzftbjt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xxfkjspj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2vruwsdvs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qygevcpn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nspuodhk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xbkvskre.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2kxeybwhj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fnzwmujo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2abiubyfp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mowhjznl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ypxckzhk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mupttogz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ykegfypr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wnxfnnha.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tftbqfll.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mirkdgdm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ajdfxyhx.html


<!-- 参考信息 -->