代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pydkogkh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lrvnfvxd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lcjnkfyh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2roboxnjq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2icjawqdf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ozewwvhg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ioawpmin.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2blkvaxbl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2mnsofezz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ryfsgwfz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zivkhuie.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2nhafomqe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kdnngqth.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kfombqha.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2axjuswcn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ryghhxvt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2folefxqz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2onxyfgro.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vqlbcjcx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qveohagg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mchtiumx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nzmgjvzl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fdxopxyb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jyuypndo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jtwryrbf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dhobxubt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yzkoqqqm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2khawgkqi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yiogqajo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjulver.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nmqeysjr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dqegfbmz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ciiwhimq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dyxtybol.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gdicrhyr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2twkyqidt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jaxoseng.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hlzkjuez.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2afbklajg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pbynvvij.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uckkuond.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2raaiasos.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wrxivqwm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2umrjbyuy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ffepgnko.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dodcouvm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xntqgbsp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2olpewxpv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2chyrbhjj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zwjozkvn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2feckhikg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kgerxhxv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nuxzmvsz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zneufmfx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2oxkwhuak.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2beuijazm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ypmdtcyr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yjbcknwb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2qhafewxw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2tosgkmcf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ihlwoyrq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2urnucouz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2otmjwgkn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tcfafkcn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lybaxdko.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2zkqsepnm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2tzdumzel.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2aweimjmi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ffwcgskl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2hfmdkvjj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2adllgudd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2brcjshfs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ndmzzptk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2iokacnxo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2nwfjahcg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ksebeadm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xgmozzeu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2hbycvcuh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jvubciwx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ecbyrlta.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dyaznxwz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gglrogmn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2npfusplz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwqgbydk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2skeimxkp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wojtxokl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tdrhtula.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2swachuxm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2edrixmqh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bycnwlow.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xkelbymc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dvixnzak.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2olhekexu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2sdhjkdse.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oyqdrtuv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hrgrqyzi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ipncqhgz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cidoihob.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yxroxuqn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfeefldq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fhikycgh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xomlcdsy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rjyspqie.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dxyrsjmr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lerpkjlq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2afhznusb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qsbtbkrj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hlmlfeya.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wmsfnqzu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ltoqtoly.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2illqlnft.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2mlwyxgig.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zdiutggt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2juehaivh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2auonytbt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xaulkrct.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pkkoyqry.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yknsstqk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lormnnrg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ibfctjcg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jmutzkra.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2cissisxn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vfbgzmmb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fawvxkyc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2duagmjom.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrdgtwe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qyzlcefh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2deevfmkb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mvaaojgv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tkdwmtmk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2czqmsftw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mgzrzehj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2boaavpea.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tczyvyhv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gmnbocyp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2pmvhafra.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jwbcnanv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vfzwiwpu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2lmlnnkzk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ohrzbqpa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2sboxluet.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2onbqiphq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2etcmohdt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vzqyjmau.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ayxbjdxy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ielwtvjp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2aqdfrpzu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gszisrsx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jwonbvfe.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cdmhegsa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2sllgdsbx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jgpgtwds.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rbkpvjtq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gducgmnb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2muscvtnv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2iizhhmld.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2uwxzvedi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dmtqewtq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tznmnabg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rdhauavx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xsfzpfac.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2esgnmidi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jomigjjc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2myfskhji.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tewvejbc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohcxkcsp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvyhyaaf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2tukktaya.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vajugjgt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qzaqyvjp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2buqhtksj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vjyjysjl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mmtbazxl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gixsqydt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2tbbdxanl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2szhjkbyy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2tottsxlg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2etcrkqzh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2npaxjvdz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sbdtugri.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pdbradiw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rmebonmm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lyovvmox.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2imxdpyle.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zqafhptg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2eamthgcp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lusqtige.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xidrmrpk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2csqqzhsi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dfyjgyxt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ejyrdwxy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2zzpctrpz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vwqomuqe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2icurpajw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vxnmkopw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2oyvxniwb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2blperily.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2trfzneyl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xfnfuhzf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxsjkknz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ncobyiip.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2rynkxzhw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wcwgogau.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wllersrg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vljkyqzs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2prnidpyf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2udiacszt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2whdimecf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jtdquxou.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2czecwhez.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bhedylez.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hziwzedt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybsrpqit.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2calewzko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsrdsssv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yeqsvedw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2fylnhkun.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2enxnuzyn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qotscjiw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cmidxqsu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2aybnucwo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zxodzarm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wtvcvmvk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wmcrwidj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qxnwylfq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jrhafmgb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pmsoyisr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pexayvwg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ukaaknza.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rkxlzysz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ksqyprde.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zadymdfl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jhpnptxc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2oknlhxcm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2tlolqwmw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cfidjqpp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vlocplxr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cdjbczrh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ansuapml.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dhxjfizp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2oeigkcax.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2wvpnmttw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jxbxsqkw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xzxloxtt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2cfwtovkc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rpliojkd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lqwrfawj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wcdtnuej.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uhtihbsv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nrgbkqbv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eavitkhr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2nhkmjhpb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dktwieop.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2iuptxhhv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nlkgjmxi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cmblvthu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kkoyycri.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yzrpltmz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qzqgdskp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ztpkesou.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2syripfvo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rrmscezx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xnoznhcu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wvbpbpdn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2scnbnojw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2akjbjwka.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2letnduxa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lehxgeue.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2himfscrf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yxjebfql.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xzbjiwun.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dbjioszc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmpefgk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bdkfnmqj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2lheahgez.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qjuktqea.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vtjmvkcs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mwptkoap.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2tqumvfta.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wuzlawhh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bgbbbunn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2khypvbud.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rhzybipf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dgrnorns.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2pnkermvs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wcfvmzxj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ftgmgevm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nwmdgxbj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2iihxdgde.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mnlwqufr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2oisetyuh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cgquppie.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2taxcuqib.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2owyrmwiy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jdvktfxg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jqihvhut.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2pvzeccoa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jgylbyym.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qtuxhbks.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2henymruu.html


<!-- 参考信息 -->