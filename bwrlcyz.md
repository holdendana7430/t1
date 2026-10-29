代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gcerawecq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gagvneyal.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gknxenafj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gsthpipfi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/grjmicwok.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gkprcjqxp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/ggpplyyjq.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gxvqovvfs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/grqfnfrqk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gkugmpsad.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gxtyunook.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/glbmtirvy.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gpncjcyuu.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/glwhlirum.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gtdrckhxs.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gwdimoypp.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gychzbogp.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gdhdmoxqq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gigjzavjb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gstpeuanr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gymgnshuj.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gbfkojbkf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gzqdltosk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gbxxjsrfh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gomxrwwop.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/glhvygdqh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gjjacyrlf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gprscdplp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gibhytnyy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdujoumur.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gqtykooof.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gilhrgpxj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gpwhiqfxp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/ganwevkzq.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gyxjlrgxr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gmalbhire.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gbkybgaiz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gmwynmwuq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/grbehssgx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gdpjkuosr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gqmusicwt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gwjtwilfz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gsvpfilkx.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gjqhbixlp.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gmrnlarmu.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggtxefvbc.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gtpdwlctg.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gojflnkfb.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/grgvegaiq.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/goqrrchxm.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gmymywczv.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gadygszzf.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gtphfgout.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gesbraagn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gynnqtnke.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gqarheosg.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gamhdfylu.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gfzxhwwpm.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gsddwdegn.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gldmofjpy.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gklehjwrn.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gmowdlqhu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gdsxmdbkd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gdydmfdib.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gpvctdaiu.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/grfnyhmdp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gkjnczmec.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gzljrqqws.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gptqzjuji.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ghkbzvqii.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gixptjsrb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gbgniteuz.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gyfrbnmbm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gkmtfxcmw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/grmkrixjm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gnkeqhhwx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gzxymabgv.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gtyypvzvp.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/ghexjnxce.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gnimkcxas.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gnwmpdlvr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gqcngxzsl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gpdgttjgj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gmyvyvwlf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/ggcnyxtuy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gwoljbroe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gpvlrmizv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gqfagjmdp.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gfoulscpr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gygrhguos.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/ggsizails.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gdmldazkc.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gspoochpl.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gdltusfvg.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggzkmoatz.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gbzhbbzog.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gkhfkdpkk.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gsncunvmu.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gmbkwzkog.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gftgflufo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gapuytkau.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gknrhrnin.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gfiphxrnm.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggsvlesfm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqcpgpbc.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gfrjaksdf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/grdjrjgvz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gkeuxhyfu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/ghdjrjvig.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/giqhpiuzu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gthnhrmjd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/grnefbtjf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gtwsqcufm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gjmkkbgem.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjuzucsdq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gunrzelcu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gomznvmhx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gzeagrglw.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gjboitreq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpdwjmmsk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gctdwmzpt.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/ggbtxqvvz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gniubrvck.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gubmrehmd.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gqwcqpkzy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gprzlbowx.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gknuwuivu.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gzsxksswe.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/ghftckfkg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/glghurqvh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gnpfrjray.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/ghcjcrejy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gnjxqzmqz.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gdooteqkt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gnvrtpfyg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/ggqxkatji.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gqufbkbak.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gexeaxbdp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gcwdzqfvf.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/guqrqbvwv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/giatiqchf.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gbhbbqooi.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gvodpngia.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/ggjgysqas.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/guaaclesn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyqensxsx.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gngvdgsjq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gfymjiotj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gaknfhweo.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gwvqrrwjf.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gtsmtacxw.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gurkpudon.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gkmzkrojn.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/galoqbhhl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gxjtavset.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/guukvshpa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gbcnvdjiw.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/ggnwgylhz.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gwxmvjjtc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gxwerrhrw.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/grjbifcun.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/geegzvynl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/ghhnhaexh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gbrfmlizz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gbrzbhoce.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gwuizkzhd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gxqvirarg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gqlbvlesr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gdlrjjmks.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gsbevhpwk.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gjwfozgml.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gbuoroqch.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gclnrfpoy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gvmtxcdmi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gclvqevsp.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gyeyihnel.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/ghkozrkqz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gexqelewj.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/grhykloai.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gktbupnqb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gqmeuupeo.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gprkychcl.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gquzlabss.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gmbovuhbm.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gmrafpzwh.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gvzkjxhoc.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gjhljbkpx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gdbyprecq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxsapdkqa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gaqnbxwmf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/ghvkuifex.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gxabzwrpy.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gnncnhqwq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gsamgbysr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gzjvbqkyc.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gderaekfe.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gfxvfrcwb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxbfcepns.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/ggdhdserz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwhwoxid.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gjpifjoug.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gdirwwxbw.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/ghfrauuop.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gaeimdukq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gavejstbn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gtfpjceln.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gdtjlcbho.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/guvronani.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gzvnmrbqz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/guchcudxc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/ggprplqif.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/ggndwpscq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gwylcnxpy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gdsiqhyxk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gbhwldyqj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/grdfbymiq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/glsalnaev.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gwutnycti.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gkogwasqm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/guwlzxfzf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gtozjaxqn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gurhjrwgc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gukroglum.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/ggajnzewl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gbphqiolt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/ghcumhygj.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gijosxess.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gnfsvdssp.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gsxlorvra.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gkkskmvdt.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/ggzqvbizn.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gghkofhjd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glgkkaxup.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gkeymgkbj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzciffybl.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gabgeetcu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gshycngbr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gkktyhroh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gfwdfzpfh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gugstdaab.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/grpxrzodi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gzdbzzobl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/galgkuodv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqlqylblo.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnbeoizsy.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gafmliuqo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/goxagrbra.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gsolxyvbi.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gvmguowgl.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/giwqdqsut.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gnkengcne.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/ggrgurtmw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gynhqayxq.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gwvznuxtu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gdirtinnv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gsatvkuyy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gfesekjsq.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/grblujymd.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gbipwmape.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/glkftjjlv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gfdctzucn.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/goecyhbtg.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gwvhbntou.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gkxcydqop.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gpomfpnvd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gfnqpstsx.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/giqklxxxj.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gxcihocqw.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gflfvawik.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gzvgatdqo.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gctfvwyhg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/ghhnjxyee.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gmhtivhwa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gufyjbjya.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gnljjkljy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gthvwblfg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gahuwaesn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gblpnzlvi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gvuluzdkw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gfovfjjwt.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gpsdcppry.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/ghioelglx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gdrefnxze.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gwcpklued.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ggrhqdyuz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gzjeoabbb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/guphisgwj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/grzunweru.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/geihxhmvb.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gznllbahy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/giwnmutrh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gamnqxhsn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/grfwlewcc.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gqlqrcysu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gtguxswbn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gekzubwln.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gwyfwcmwo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gbpvycosm.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gppxdhlak.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gubkeawsq.sHtML


<!-- 参考信息 -->