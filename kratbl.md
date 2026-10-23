代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vhnurjve.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3brgnjmdy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3cgqejtzl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rjnoesig.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uzefoeks.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kuzknkgl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3irdcqdwt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3njakydtj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pivltita.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fpxqumar.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ziktoxie.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mwruvvlw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cozrrbiv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fwddqybs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ikqznior.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qbhmysih.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3gypxpnhj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmnwdib.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3dmsvultu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vtjbdsnt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ilkvyyyg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3efofuicc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rgpqhqas.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cejlqnpi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3okwzjrrz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tconmbhn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nivwcgie.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3fvfrotzb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mkycxhat.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qvbghrrx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3xodoutzn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zynjaaxp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ortxisjm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3bfeyaavr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ielspyol.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cthdnvwm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jlamwoji.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xarocpgs.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lpmievmo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pkyquuvq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rrsxakmf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3tuyvxulf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bdppasxo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3uqybkwbc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jbondfme.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3epxnupkg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ukclihgm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xylbunne.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jkjkqeez.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3awwlfobd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3droeuwgr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3reochmjz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ijjvuuzt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3thxlrorz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ubdmvijq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ninvlrmm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3iomcltmm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3pijuontm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3pffbmhgs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mhyupdaa.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lxvjpbsl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jbktthje.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ckshqysn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kifzdpwe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3suvmfjxp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nndtsptl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3puajhmkp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uqjicblf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3eptdcdxv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pznulbki.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3aeywfgqh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ilrxvwwr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3dtcvngew.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zgmebgxz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3sjtmnmkj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kllbhxta.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kiexvlrk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pnaoremq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wutockoa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vgkxjgur.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tuzjbaov.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3newdkfpf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ekpxxiyi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zqqzmuag.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3pmatavfl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3twelqopa.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qiuohhuu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ucxxpdzm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3twwtlnqc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mganhwws.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vzdknyat.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3getsfqec.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vlztkkqm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wiehoeli.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hkzhudlg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zwsmssbp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bqbphxsg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vgnnivbv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pcrnvrby.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gthsdukz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vngislst.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3wpiczedj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ttrmpqnv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mwyuvedl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3chhvesnu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3isgzzjjl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ktlnjakp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3pqiihfxz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bbqfnkpz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3yyulzxxh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jiznpvmh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zceuxysp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rttdomaw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3nkwpsapn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mgpwfbgx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mcviiaga.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3owjizmra.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3fsgizyhf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wisnzdju.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3exlztzro.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qrfctupd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ysxzhxje.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xoraldqy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rfneldlw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3pczvzdcw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qzmznjnm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3congginx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rgfekqny.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3cibqsqsm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ospmwgdu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3irodqulm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wgxohpcf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ppvyssow.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3oxnhmmrc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3sywqztpb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zdmkdxqy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3idxidqrm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ipxfgpwv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yboaicke.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3afjouvwn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yozhsbgd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3azzpvubg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ohguekcd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3kyrrdrrt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3gpwvwjhg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qelzejnw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fgalbifh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3lksateju.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bnrfadko.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ybebrgji.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wkmyrjsd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vvrwjqgt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pnbnkwrt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jknygcij.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tnybjhbk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ixefbkmu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3pcbsngsc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rdyztjor.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3omiymwda.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3imvueski.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3idaublkk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dlhctxdk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bjshtvws.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3shalrcam.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3uypyljxl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mparsqpv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3yxeqgkmh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yuucsbzw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xwyukcsw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3thwsmhkd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wquvxvvw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3aykpayjc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ndwsbxkr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3uoiqzcxn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3dpxbjxlg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jcigihpu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxwajmml.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3evstadwc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ihuhuamr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3jypvludv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xnmydihf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hrpoksju.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3qvmmmpfr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pyxpznkr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3iijtfslo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xdmvgyre.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ipstbdjm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wmuuuplc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3zxqtfens.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3alzxcaqt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jgtybity.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ijowjelv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zcrloora.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ujkdrohx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gwugwulf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lwfzskkh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pjofknpw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3spynqrnj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dpcxhjov.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tbbknnqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvubshfv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3hlyphlcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lianvymv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ovgnkomk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3iofupygg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3eoxhrdnk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ednnngeo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3giemrgrm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3mkhcfdhq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uskuumnn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3wfblbfsy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wuxtrtqn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3uumqqbir.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ibmhixby.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tqybjtkb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3upmnaowi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hkzqrabk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3apugmkrn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nnrzzhyt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gerfecul.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tsfvipip.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sjshswyz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zdjvclce.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lzodhrjj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nmfmpjzk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3celxuiqq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wxrvdrwc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qqkcsjxb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3kghaotll.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3smgfhkfi.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xjczfvah.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qddecmxi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3cuqukcjh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ldivbnzg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ztjhwewn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ocihdtfe.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xqibbnbt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dzbzxjoa.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3clwqqtlc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zviisolm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3oewzohed.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vfgelvrz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hbcmyzoe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kvgzngub.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tfpethjg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3iwfyjati.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3tzpomwpc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oxcbwfxu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3cgnqhswm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zhjnndtu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eygbbfwu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lltetbos.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gdahpenj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qzvpjehf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kwhlreqo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oayufssb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qadyotca.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jsrpgpfy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3yvogvptx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ldtgwkqj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zxocwgkq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gwhbvcpp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3woqsomsi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bovfqhqk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hyzbijby.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wdadagio.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xyakkczu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dwblslgg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3wssrboez.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bncvxplt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hwcvelal.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xaqtmtso.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dsdgtsja.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cevjfnmv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yteowkkv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qlhcyvwl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rsdrubqf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nhhdqvdm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ytjrxmvs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xzctbfor.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xbhphgda.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ynzvdydl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3znscvjzp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vjjihldm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3usxkcvzp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3akmhsyyn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3whgsekdc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tyjkvubb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wbtepwou.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3osmiwovg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3drxlzpjb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fmgckpqq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3fbpomlzm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wmkrgpes.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bqlrulor.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3apiybpxn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lpqnrfmz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mnqdoktz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xxjsqvfp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3byilrhte.html


<!-- 参考信息 -->