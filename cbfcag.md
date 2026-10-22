代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ykdryggc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2quuubmzm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2bhqzpwbr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qveiivkt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bftzjtcz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fmawzvxt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ckatcxuw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rdzzpuqa.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pxodvcxh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xwnznncl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2hbilqbvf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hivxbaaw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fmksbvis.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2sdxogsjg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dhourxxz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2txbfenlc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2skeevtys.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vuvbbgln.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jbuttwih.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bxgqbzjs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ljsiihnw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2slcruycz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ovdjnaoy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ilmexyvx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2igambvkf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qcnkhnoa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2albaslfe.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xhmltiid.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hououays.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sfsxpvww.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tanhscst.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xwmgjptw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qrncqezl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lvjwygix.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uqwxrxpq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xlalxzfq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jetjjewv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2frkwiajo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2odoksmlw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wthpvxts.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wihabmcz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xyiheuvd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2swuqgtkv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vslaxlvo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fmxmwqxe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2dvcamiyd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2poajuouu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2moejmquw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2qycgqlkg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2npdlnvuj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lwjqcpwo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bzwrylcs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aktyiord.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qcnpvtbx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rvuwmqde.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lsaaphdh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sznjlgya.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kkliaztk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jssajavb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ponvwcvz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wpwvqzgz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2larrmysp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kjzgeohd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2drozjuyl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xvtrgsay.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2frdxenjx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fkamjbcq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pjsdrcmf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2wcywrlfk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tnmwxxkn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2siryhxyr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2jniwrcme.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xrcstxlw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qbzpquhb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yadrtpse.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ebryxibx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lmehfacv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2upzqbxrd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2cavmcouw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ripgcpep.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qtnlrctp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2eppfuxyb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2iumfncsc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xtkmeevi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2amjirnsq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jvjnstys.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wvkaariq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xlmormyu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xanascge.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2odungthm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qyjuifmu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2gfbvypks.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2cionbdgz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rixigcvu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pikqqcar.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ugpylmvb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2hugjvriq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bnsqjtjk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zkzorvjc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mzyzxwoa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gbajvxsi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wcinezmh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fjaxpdrb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jyjfpthh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vtydxtjt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tkfqllrn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ytodiqzc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jaojevxy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hnumgjcc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qmpaeqzg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kkeomhvd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ctooykii.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sjohnraf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vgsyfjzx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ijwirbor.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2njxosnil.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bxxmcwpn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pdecqobd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfairuft.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vaxganwg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ohwxypej.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zcuydwye.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xjumqxxn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tnseitja.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lzifwfyl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ndgeuoix.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wtmzchvd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqedgxr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2szwclhrc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2zldoktml.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nprjvhkz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ssvsjfex.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jfihwohn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2jzeeqigg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wwzftgic.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qfudbjzg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2abtxadba.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jgdwujoz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2uvkejwzn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bjueerwq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2emvwtmoi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dyftmhkr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2iplpajou.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qplqpolf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vtidgtve.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ojzvgcmu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kvqwaqja.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2neippsbx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pmotbuix.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pugkhgwj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2mnbkgknc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2qjcfhmko.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ewncvrhf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2eyqfpkki.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zesqjxhi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lslufohq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vtouuaic.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fuuhvnmy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2sqbjxrig.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nggmjdcu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2unbzksel.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2oupgcwiv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tdlrpsmx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rveosura.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tgvpklzu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sdtgnqex.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlvrhbmk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eokfnqyv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyoensww.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lewyodwd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbdvfhxl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2iorvuksr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ovssylxg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lronnxla.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kzerauxb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2nmflgaxr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2coozlvjy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wlmbwulr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kxcixtpb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kdklehsu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ylkvtlub.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ddgnrizm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2phlqrblk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2chrzrvsh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uzeoisit.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xjjgoipn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cnqsvjju.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tjeeyllf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kizjomvb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2txswtafi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2afglexvh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2optfskjg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mqnuyhbr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hqwfgjcl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kzhrgzhj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fzqhnauo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cqgbwxkv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kwhrzkrm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ksdcptqd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ufyhgggh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2aocymtwl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2viuerawv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2kjinkxuc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gsnurrio.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2okwzzsgh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhlrjrwl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ppnxjfxo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fpjejgcg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2cnwpapkz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2diyazljn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2txrajeax.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2egjgruqy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mroqsfez.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2eywmnhnd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cittczfs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tivnjflg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypzdfcgg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2hsbehyli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppruzwvy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2utlbqukj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2wntgxxqa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gcizqizo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kvlbmxhl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xnrzsfvd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lyzynoec.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iosphcop.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2crikmuhf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ouceckzy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmcoueqo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2iiafrlez.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pdlzbapj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2psamzioh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2maftvehy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogfmwlcg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ombdyrwe.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rzztzlod.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pfraxqtv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dbladjza.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2suehnaml.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2isvofvrw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2faqmdfng.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxgfvlg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2spiusugq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ldjjduhb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mgbndobk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2iqkvnxsj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2hsmjoqbg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qzlinxii.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gnetbedk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qgcglrap.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hmrxjmln.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bjokfnqp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2sffzdypt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2boxjlnsp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dekaguyo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uwwjdnid.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2iccffjgw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2isezojzx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bvktjbsp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zwoocdid.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2igdxuglz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2rjgqcnre.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fenywrdw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mjyipixt.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vpsjnqnk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fchvupsx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xkaoizzn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2detnjiic.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jspzmbwk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xxwkghfn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2avhkusxw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2indiwyci.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pxpvmaic.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qrftpncp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pkaqlesr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yrenrwdp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2adutcgec.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ylbrvzae.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2nqfplkrn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ukitccst.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cnegqlbq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2rrrexwuf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2gictikou.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pxypsglj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fbgndknq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vlfbkvkd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cjnwvwwp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ymavzoju.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2klaugbgs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2repbgcrk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tlescqvt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2mbzaktox.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xlfphadd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kuwnydfx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uhunpodg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xxkepjbr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zmskatju.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vppoxldi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2actzpdgh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bbclxybv.html


<!-- 参考信息 -->