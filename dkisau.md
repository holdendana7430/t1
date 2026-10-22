代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zuwdilgy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vrsagysq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2uzdhzgzq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kgbpcths.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mvzwzjwq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2knfchqbg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rzwfhrag.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qdldfpmm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mqjjfdur.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lunmgjgz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2roilfezk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xapwtykt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2guhxanpe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2oijwpqjg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rruzmcje.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jljhoemy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2aemyapil.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2miimzbyv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uagprkgc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vsjwwhel.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2omawlexs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vjsixxja.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xinfwkcp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hsdgdihm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ycuaylrk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2voxlqtxy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ollqyakj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bvorooym.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2twxereby.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lgbtmgvg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fvaxcfwn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fliutsku.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2pluxwxeg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2onzrgqux.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qhfpwrxb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qldsimbx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ubdrjvjs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lzovxmfj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2axlzhgxr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mgijkrdc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2acxpkwmf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rzgcjzqx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2obltdqvi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kfyboncj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2maitjzjw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2osdqdmfg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2uzaidnkz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2sbyylpkv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mirkhvnl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2afhpoixc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fvpzaoeg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nlfapays.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xxxwfhdb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qwvftogg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2opmptxkb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jwpnxapm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2rjprllxe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2bwvgjugx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cqdytmzv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2orsbpsdr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dfynbyxg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bhlovkyd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2caxktbcu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iqzhqrmd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zwwwfnnc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ncoajjeq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2agcokanw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2worrzoii.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pwmwobmp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vhywhicd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2sxhozkjk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2stwjzmzz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hryatqmc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2lmlzkrtb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wzmkjpzk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hupbghxz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2idcwsxgr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ysivkqaw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qdqxepdh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2humizgvr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bfsxbuna.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bljibumd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gmzqipgd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2vbkaxsvz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2forbsunn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fumepsck.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yvghparf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2laelsdog.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bgcksije.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kxphpoht.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rbkvdqet.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mydavhdb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jvffvdbd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dgohrhif.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hqyirbnk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ubdgqagu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2skqnbtrj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dsvkpvfq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2trkjxnya.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wsvadsxt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lfbwmuxc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2chxqdsos.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nfbswhmj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2seekkrot.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hnkcfnsv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xpkpeqly.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mprjdbuu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ngyltqpk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rgdvpsbi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ebeubkbh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wyisegan.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snmiaqmq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tfytlzvj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fxjanznw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qiltubif.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mtrptwft.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mufnswmj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2vdebzxft.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lnpfizua.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xfxpexan.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2yfosuybl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tepgzcrw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dhdbusnf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2jnwibwzw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2gbcelrqc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vnbzfwqo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wggijqyo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wdmivhdk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nlzwxwou.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2fshodfdd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gmkqwdhu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ndneuujs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xetkalwr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ksbspbvp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qplswjph.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zxlwxgqy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2drnrinao.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ipkgwbgd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bylqhark.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2josnonku.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tuvnqoeh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rgkrfbpv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2aniyzxqs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qwsvchqm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2lmfayazb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2yhhndtsp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2iuivicin.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gwbdtimf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ppalqcxy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fjavecka.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gzwinwka.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2htvahdgi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cdglzhpz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hdidanox.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2owswjltb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2knnnygcz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2opphtwkb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xldvehsu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2hcyjmxsc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ahlycwhq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qzexicgq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pwiacsbc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2prlvnfxt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zstppira.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2fewmmftg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2izjldubu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yfdczrhy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iapvvbvs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kaasachf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wjpgfxqs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2sgfixzyc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2udehmmwp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cyzruqin.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2eljvgpet.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iudiwxzu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fiaaieqi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gsrbleat.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lqcnuctd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tworcegw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2stoxtkoh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2sgluwvpj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kjazmgtv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ggjbyjrg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tfxwueqk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jgolaowk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nxqvergp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2skxtarld.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hswfouom.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hkcxjuev.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2swqcofpb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rshxjdun.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qawuyknk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2oqzfcjxf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hgricony.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qicpyrsb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xxcipygo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2agjjrrpz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gaasmewb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gtlgpqhe.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zpmiviyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcabvkxq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2heubpytw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbxqdspg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ngguofjt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bvrnyknd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vrutdwhs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ahxjuykt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yjoxhxuk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2csyaezzf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wvmhyspa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ureowxrq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2alkbmewl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2pgjxahuu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pvrovvei.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2bapikjqm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2myhxstdm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ysyviwct.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2raxkkqzg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rafevqqp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jlsbezaj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bdhbygpr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dcdbadxp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jqxyiskb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2myubqxzk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sgoeubnf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2crovrflo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lscjvaob.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zxuahqly.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vsiipkzt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2acyrgsyb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ilzifjix.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2twbrlbpb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fapfynlq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bwpmnirm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jaiwltlj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dedforof.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ecnbctzw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2phewidrw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hkblgzip.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qcbzpamt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gqhusbet.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2hlolpbtt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ovoenzha.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2khcglmlb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dsnqtqoh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2tqgrhoms.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ktoumfrt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mjcxbecl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2srgmyjew.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2smgnebgb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gobbmoqd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jdjkdkou.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fwmprpln.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vgprxiiu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kojypjzy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gdqlrcwi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gucrydec.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zyibqrqe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ylnlkyno.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bosejwul.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2sutqcycl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2smrcioob.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ahuzczdw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wpaoacej.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2oatinifb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wkuxzxva.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2viqpfjai.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2nefovlht.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gfyinife.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2igddwgrq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hdfcuxdw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xblvkmkh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wcqwtmru.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bpqzszes.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fonvmsra.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2znjrbjlc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hypzcoks.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lzdnuojm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ueitqefw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iohevbnj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2grbiqtsh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2knvlaszc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2udlgsecu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2odiwytbs.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nshlixyk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sqvqtluw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2xdpqyfig.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oxnpfina.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ozeferxy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vrilhhkf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hzhtgqgx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kbjcguqv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hyzqxlwc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mzdbusyc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kjowtwmd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qrvlgcju.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xrzgrnxv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lqmkuyzk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zkocvqtn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lqyzxipi.html


<!-- 参考信息 -->