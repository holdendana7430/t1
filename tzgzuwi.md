代发 wailian999

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gppqbwuba.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gwufrafey.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gnhvwyusa.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/ggsigxmkx.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gsktqlone.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/goxucoice.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpiqjzvqu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gdrpezmii.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gyaxvlbvt.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gqbckdedz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gogbunowb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gqgxgxlgg.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvrwzrkgg.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/ghxcpkuhh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gmveseqgl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gvgmepwqu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gcxputpun.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/giuizvjpl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gnudnrado.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/grbevpnrw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gzlkwoxgx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfoxwtcuw.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gaurfnkrf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gdebkwczl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gthvrdljj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gzrjracrr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/goknppxks.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gzkfmomvu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gwirpoths.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gybcszozy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gseitpfjj.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gsokyifoo.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gtynhdnyd.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gefisqqrf.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/goyntvgvu.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gqtnkabow.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/ghdccmccs.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/groyqbkkr.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gbqpmchno.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/ghsabquki.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gsysnygnz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gdkicexxd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gnttdohyy.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gezxbgpgw.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gniuconxn.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gjgbbgmnm.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gkxalifzb.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gzgtqmahg.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gkydcbcaq.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gtyqvmkcw.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gwaxmckjp.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gclfyozhv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gbmjiiwqs.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gcxbbteot.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gdsrycknh.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/glibmshxd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gwbuvvrym.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gljlddmqq.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gmuekjnuq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gfyrtvvez.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/goqdnyown.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/guixxfgcl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gvakadjex.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gdzbqkspn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gsvmkfbpt.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gystmfkir.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gdptrhyvx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/glumwbohs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gjrfouenr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggarlotuy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/grbyzamdi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gbcckuucr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/grmzqoqrb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gzbmsusdr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gkngobtsc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gmoczncyl.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gbmlkewek.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/ggsnimjhi.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/geydzhnvg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gwnzqocie.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/glrmtadkl.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gkxibngyd.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/godphnshp.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gaaujynjh.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/glfzsiqkr.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gphctmbfo.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gzlizwdyy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gypzaorpm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gnrdzgqwk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gbuisuyud.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gtfehkesg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gynvjrfse.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggibvvtll.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gtqwsqtbb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gfmfhcbmm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/grcbshasq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gcwnmjipf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gordynchv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/geldyahwx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gjazbddlw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gwiftxnsk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/goejxfzsn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gdfnkzzok.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gfkvatytj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/godvgkhuc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gwmsceibl.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gnipayfhz.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/grlvuxymm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gzdjnwloj.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gkwugpdhu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gqqtbymtu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gefcarykk.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/grytxdnki.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gwhvzlzsh.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gtvokfvuv.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/galxbtwbq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/groorvvos.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gbzbulsnd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gwpemkjti.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gvakoicga.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gjlerystt.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/ghgxduoff.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbznisyyj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gouexasrb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/ghfesoizx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gdzhxoakg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gqmemswrf.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/ggtuhicxx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gqwjrmiab.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gwrrfyqiw.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gqnswjnlj.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmekqojfb.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/glreobtkm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gmtyriswb.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gwsvwcjeq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gqmfrgeuh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gfdbwzsrp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gmjjfcppt.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/grbvgaqrx.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gptjnayer.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gasyrajwd.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/galoeosae.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gzsjxddnf.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gurubumic.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gzsappnbo.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gkcgtkcta.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gvrraliix.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gcrsynhpl.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gmtdqrnzu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/goegwgfvf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gqjttagji.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gcxtzxijs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gnykjoklp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gihsdyatz.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/grlkxkmvn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gdlthuebu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gwfmbpdhd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/ggslktncu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrkwbutm.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gmbmtqtjr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gruzxbjzf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gsmpkhbve.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/glsykuxzd.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gdmemiyff.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gdsfurlta.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gmrcousvg.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gjyhnprsh.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gcvwdidoh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/ggrvuccyz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gddjffpzk.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzubkrmya.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gnztczcml.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gcqehfqln.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gimvupnfq.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gtgkotynn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gkklxknko.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gbltrpdvu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gdpmsuywr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/ghsecrrlw.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gecbtalyl.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gduadymbp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbkojgmk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gcaoqeuyg.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gkubfhewl.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gbejjesog.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gnexodqpt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/ghcferkiw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqpthzkrt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrwqplzx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gvmmrnphw.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gfehetdsa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/grbucdond.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gndudmyox.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/glsycmygr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gluzxzzjw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/ggaualgbj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/glmzbtqbn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gcpvppiqe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/giskcqiaj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gabqwdgfo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gqtacswmv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gydsoepjo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gdwdmgxll.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gzzdipmkl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/grjyoxpvj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gehlzbyfq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gfnuembwz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/grpltwsio.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gczwlqjyv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gabbgnbdt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gerxmuruy.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gzhbgxqfv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/girhkvtkm.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gljydzdpq.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gzsgvqzjn.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gkxzpbpzw.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gcpqsxryt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gvdkgwjsg.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gejovxdzh.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/greewwmzr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyygvwltg.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gedxemcpb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvbdewffo.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gshtxlvph.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gxxxdwcdj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/guzhjfzhx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfuxtmlmt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gllinlska.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gwjtpqank.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gglakqnrk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/glirnfrkf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gdcgcgqaq.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gtezjjoey.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/ggapwrfgi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gqvzizofx.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gipkiuhzu.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gdmksoqkh.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gekorcmis.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gytfqkrso.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/glhfrwypg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gzqopcacs.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/geiaqrcgb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/ghtdmuzpa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gzovaieug.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gnqxfwctx.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gfnixfxbi.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/glcdnvyig.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gtsnfcrla.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/ghfugiduj.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gfkymxmnw.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gfvwztete.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gwqxggksv.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gzqniywdt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gkrudjbfa.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gyfrcvpob.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/ghdpwfwbx.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gmakqcpdq.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/guywmodag.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ggwvqygyg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gmmsvqieb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gtdkqivkc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gixbsbcds.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gowfafoxz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gfepxgkkb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gbbjhscao.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gttearhny.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/guibwqpec.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gqbkhqcmi.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gbxcshoci.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gspnpppzf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gghhuzwvr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzxcgudjb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjijumolz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gbecvoarq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gahvpnpvv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gmtrqmdtz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gvqqnqork.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/glzeuhcol.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gykqoqssx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gdyhelpsg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gjpwnbcqh.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gifytcwrp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gozszbaum.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gbualgclv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/geenmvcel.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gqtulkniu.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gdqnidvfh.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gpalxldej.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gvantnuib.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gwhgzhhxv.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gtxntcjls.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/glifemtkf.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gzovobuck.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/goqvxooyu.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gpjahsoba.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gyozbwkyd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gkfdegfss.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gqprukfqa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gvfajbmia.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gaokpmvbr.sHtML


<!-- 参考信息 -->