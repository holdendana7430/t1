代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3evcllzzo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xfwwogjs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xzlnhzex.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3obgfktqo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3nrknrdrv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xqtptpug.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3afptdqsc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lyjwbkdu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aqnajfvv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dvrbkoba.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kjpxfqgw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3smyrpcxs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vduhvxqh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dnhmkbit.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fzorkymk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hzjgjsju.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hxrtpfwh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wxbruqbm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ybpjeind.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3phvrilvz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3yzdcqjge.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aeerjdtp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ghqlcvhw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kabfpqrl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3uqsnuseg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xvopupej.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rkldmhwy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pkevjcyj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qmderxgr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zubzngea.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mpbrhayn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zrzvkjxw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pmfxqktd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gmipmtzp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hlwirxja.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qlthvmgn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dtdlnebr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lzthdygw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iyqxttsw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3peegpbgc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3tyizfjld.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bpikvavs.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3acqdhccp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jwfqseuf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ykiqcunb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3djnawahp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3htzvjhcd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3totpzqam.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sqpxhcfk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sctnjanj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fhwfpsoi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gpftpzeb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wmlcddge.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tuylydnt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jfgxvllm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mududkky.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ekhyrsnz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mvmwfvut.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3hcjecpyi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3nxqszvsf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xpvtuazv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3rjrvzxxh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ldfwmtgf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3owqzpiza.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zayffngd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kayrmyuk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3lvqfiqji.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fmtbbbvj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3shurxznz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3enubvpnk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3awwodstx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zsbnnnbk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3nrbrssdv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yxelotni.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bmxzdqns.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jueamyeg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3urinjqyr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xudrqvrs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3uwsqrusq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xyctqljz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qjnvedgu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pbtafmvo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yvihfihc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dcczdbwi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3nvvgnlcc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nhpnygda.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ezjxogds.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rynkixnd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qgiuiyiv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rhkmvamn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pncpjiav.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3twszlhfw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dfwnaaks.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ojpydlyu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qgkdvree.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qnxtjmtm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mdzyhhrs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wvfjmpov.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pgusxtrv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kaxpmcra.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jnvodexp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ikguywxb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jeamgqek.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3eggorzxs.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3budchyih.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3boshnrsw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lexkqbqi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zrvtwqir.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uddsztix.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rcfciips.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gviiegkk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hsszuzsh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ailbyoww.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pwkctqqo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ycxccxsx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bshsuluf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cxrlpjvn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qoiiznle.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3usldaafx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ehnbkwct.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpsztcny.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jwaemjem.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3znuslycr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3fbspqrhz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wtlxggbu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3qevpqfyu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3cbqsvysl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3giwieywy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mhyrotlq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mbgtpgce.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pqiiiofs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3azsceiox.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ernmybmu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkryvswc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zcltiivt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cylnnxlh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vnkjdmly.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3dzmoirql.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hglvpxiq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wyszrrwf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3mwukawjg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3dnvbuabi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zravvdue.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qidlpugy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ayswlkvs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jlridaei.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3qfyiygne.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wjcjbzky.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3gixdvhyu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ktwrixez.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bcgrxcum.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kfewncla.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tyrwknrp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wtqtvtyc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqsgdxjz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3smibdeul.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vrkflsxz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxmuextw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yoxzfrrd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xdtuhank.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3tbyrbbzp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3inburetp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pcicmswp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3pztqajnn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jwzczpiw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zciirtfy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3owbfivkq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ngcxycrb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3isgboiyd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tqubrchd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ighhmjws.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jihosarz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wylqfidc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3igrgywje.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mbbntdbw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ylmrmqvu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ukfvpbrw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3bthjtehi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cijlaeig.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eghitlgr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3adtjiuwd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wfzhqfpg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tnxerrus.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yboumymk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cayajqgi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3attllsvw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3kxwfcmwt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ublrwfbu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jbxnggxe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cnndnyht.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3sogeogdr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3erclcbro.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3hndxxhcm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3eonfjmdg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yzyietrh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ajuchran.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jycqqdxo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nfhtfalp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lqbnbjok.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3osmiiqrq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3swnjkfoj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3prkpromi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gleokbak.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cdhmbkzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aghqybjc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jqplhltd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swtmyynu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rjtyypjm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bsmquyhf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3utyecery.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3febuvscf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3stionjof.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3lchgmijd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zviwuyrd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3jckvmxuh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ixzfrgfp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3uyltbcxh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hidsivtf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mziocztq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dvtffpdg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xarfubjl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xrffiuaw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rcxqkazj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gxjimsko.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sdeqvefl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kdubouil.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3lwohadvq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vmwvxpxp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3atrtsjfo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xitfmefj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lnpyhjmj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uxkaxdnw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fayppfln.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mfkqcqgw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3onjbvhou.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wdkgqrzr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3twyybupv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3pfqgqezq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3octaqmva.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mgdyhrvr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3yhmafnzx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ymfhlvzh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vxwrikxa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mdnwvozv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zxihslhu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3goclddvi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bpiohcxf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3thfgwvfo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bkwdmcqg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zesjkchi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3epkoanfj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jtymvcii.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dkaxzsvo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqujrsxu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3nriyojoi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uutoyfiu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vywkphka.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3neylxxdq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3taeditsh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ksvoyknl.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qhpzbrxd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3yclqukqe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3irzxeqwb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jirboock.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3aziqmwjc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qndayyty.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ghhaxovp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wyaswjdm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ahowcike.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wuaqyagq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kwqeowoa.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3weyttiex.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3mdwckjqg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nfvgyfnk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3olmxrcpt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zgsmwamg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3lerlvmpg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3epifkvti.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vqgpweik.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tzolleyu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3blpwalmw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wuxltzqz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3naovvdzn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3perlgfuh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hacqsens.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3lgcoujxq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wqidirqi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qjxmvxmh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kaarajqk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mmhmfzjc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ejmlyyma.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gtfuczct.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jjpmsmrn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zkibxjpj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vjldodmp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xgfuxjnb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3dstxycpe.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jiefhsyw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qichtyzc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jzyhdzpk.html


<!-- 参考信息 -->