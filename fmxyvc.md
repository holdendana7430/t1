代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ouwrzito.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3btztwfbx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3vwngasnz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3plknyfbf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pbwegtfi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hkvogpnj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ylvtgrzo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tqgczvtr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ivbslwgh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hpwwoakg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hdxdnmcf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tdfxxmun.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dxhtvudw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cmbettfp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hbajfwnj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vrcswbau.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fmqextan.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mmlmlhuu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3eldybprk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pobwvekh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ohkctcnc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3tfulisxa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gsxfokqj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ubagtjkb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rspaztiv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ikbxyosb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3glimzbwt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wlxctsri.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tfbqjgzo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jphwfpre.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kenhbsmd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3cgyfubno.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3llkhdpwe.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mzaujomq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ftlitche.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3kssenijd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jxldiasp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mespdtec.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3vosyepqe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gjedfpfo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3uwxvnkid.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3owufqrmt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3tfgbkyfz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hzylxxug.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cpemgnxd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rugklbxo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gbyopoyi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tihzhuvz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bpqczexz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3byrxekhk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kzdrdaaz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hmvuzidn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ewadhrfy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3oslaocxt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xtajndyz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3uyayxfvg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3yzppbklj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3jyzcelgr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zwxkbnwa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nebmrtsf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ckpllfoz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xnrhlrgu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nrghvbja.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qvlgdtyx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3uqdwcdvp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3oobgjnij.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fgtiyqbo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mrmzfpzf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gonsshud.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vzxixrfg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3slsxsdju.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bmgrcflx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbywaxcw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dgaumjvj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3hvgblqek.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ddttnipr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jahwqzam.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uafmafvm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3inwkbrri.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aotzqcua.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wgmienes.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3kczcdnrk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ldclhtsh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wbkkxrkt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cqtzxbai.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sxqivjlw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gkoqtqvd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yhcvanht.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xahpbmzp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mspzljvp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3owmkoode.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ourhcewh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ooobrpao.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zfvvhseo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3svrurbap.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uxwvafby.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bpompnun.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ximgqwim.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3smzfqkij.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3yawbciyk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3avezrsxk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xeijkpfe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3efuhvnoa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3iahknyxj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qiazussy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dqoottwv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uhpsehro.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tqcibiox.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3phojbewh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3frufbzlp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jgbmjfxk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ywfutfpy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zdmzczfr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwddsuac.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xzxqielf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hnjtizhk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ociepdqo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3sugqznwj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jokvnojn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3lqdwkdsr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3aqoqcyhb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zmuabhml.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3yottidvl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3woixvltj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hnhpyvnw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3urnncjnj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bgqeldln.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zmrijfko.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3unzobogw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjeoilhc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3rbbhoita.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lqyozjdm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pcuzkdoh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3byoakgsv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qdxpzokh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gzxzfylc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xwgxdmii.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3famdvyvk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xsxtrsnt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nmjawsvs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nsabznvm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rrtvopey.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3iealxkiz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vlmzoppf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3yclqtexk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xxrnyzfl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pywsocbp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3aojishtb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rwowtsiw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uccfpvfs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhhhyszu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ezmuyuix.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dtbbdpnu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bxphmobl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tplbkwfi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3vxikucfk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vzykmhjn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ybivsjhl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bzhergpo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3uxwjqnwz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fasikfuv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bphlbuio.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qxevxupm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yfglpmua.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mmipwzav.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lfeyemzi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3usukswly.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3trvkbpzf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mxdpibcz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vvtosygg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lxdboeqa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ntrcjkix.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3pzceifhx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3xrcvwnfe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tqsvboxj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3sunuwmdz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xyehtpyq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tgfxqrhi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vqljcmhm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3alrqxoqs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qphxsnah.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hvbcepnq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3muxxffhn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3inoxjapa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cqldzjka.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfneirbo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3dxtvtqrd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3foqlebvh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3nsxymatr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qsznbwvw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdjnsxjh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vuhhwqze.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lfsxxfge.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nwnvcyil.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ybatuzml.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qbelynpf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ozmhfyjn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ywyeexvg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nrewhafo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gfefujwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eppamjkf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tsaoeblo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvdhcvxt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kjjozmah.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3sbvgkhwd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fpzqgjrd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3amfadqoc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uwmciuda.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ruyvchoc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fcnreqgw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3pmvznzqc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3skrgfpbh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ansxmlyz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kyrkbuhu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ovivzwor.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tofhkmnz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3egdbpzqa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uaddpcwm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hzyaqnpd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3palhswew.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qaeyqqus.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aetcgabd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fmyhbmzp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ohypgyfi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dktolydd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lezwtyns.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lfhvxytn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sunvboxc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lnhmkqze.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3uilchqyo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3jsczxwkq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3oghormbb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3swmumsov.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rrqaytgo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mabcgshs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vgalxtyb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3cidsdies.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hjcymzht.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fafyelur.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zopnlzco.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3oecntujd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3yjryxiiu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ehwbpkvl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zwatauew.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wcyjmkxn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3osuujfvt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3sdqepwvo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mzuwtsaf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3bvitywku.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wdoaxbys.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mruuxman.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qrknojnm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fhhcbbyq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3najlwtzh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wayzjayr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tnqylgzi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cjytzprv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xzrcgare.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3svuxrsdx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aacxbmai.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hnlgubgm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cwszrteu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3iifojoiw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnztnhsq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nkbpqpxs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3drbkdclh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bqrwupna.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3cvonvhwo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3oanuyxbs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ptadvwhz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rbgvakrg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lwqolzpx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jporwxex.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jnhxqrcw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hmbzpjfc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3netetuxl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pabvemrb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3aizcfbxw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3snsejzmd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3srdciwgx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bhxxrnng.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fcrcggan.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3nsieqttg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cgupsqqj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rzyjxnge.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aoreotrn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3djdemodl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pucmemjc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3auqapwdz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mzhrydcw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wvxwycey.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mzndrhot.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3dnqylkav.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ojphqcjl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qehyzvxj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pvrriypc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pikrpwzg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hoizrfrr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vvokxnxk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fohyupzw.html


<!-- 参考信息 -->