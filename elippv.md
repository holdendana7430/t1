代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bunblbiu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rwnnmhcs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ztgqaooq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3kwianwyv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3liiqigvk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3weazktnl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ghmqtvua.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uaacandf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pguciont.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nsvzbqqh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3aqctuvil.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jelgbcti.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3idzwiqkz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zkrsnkmr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3opgppkth.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nwjznvey.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tauruulu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ltdocijc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3igmdgwys.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ioknhtct.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hgvmztoh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bwtihylc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ppcrnjbs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gabtvykr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wjtlfmrz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jkmwbtfv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ylvctwuh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ffcntggp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hswevrwp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3eepcutgr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ystcfqrm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3sdttrrqv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3gwqmylfc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3vledibly.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rhspnnnc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jxavmwme.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jvrxlaja.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hhlugmoy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3pmvaliob.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bfwyugqr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wtyblvgo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qktyymvr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3fidpifie.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lebkaheq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gyewmkxe.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3iffpxgog.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wavywqux.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3iwaemjyt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wwsylnby.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bdweermb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wfnplrtm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3reqfxewd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tbrutjym.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wdkxfmns.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ahqkzczh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3unonhhcd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jwkxxkch.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xkijkffv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wqqcvvil.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mxiiomok.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3isxtixts.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3usbmldkh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bybbqkkr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ohntyahw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vqbvipvx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3leufdvym.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ptwdjfos.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3kdylzvfs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wtoezmwk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hyuhygnc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ujflmuzo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ywyasgig.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zttmpjtc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rtegucen.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fzwtwuvf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zxsnddqs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3skdqiboi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3oumyzprd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3orlasewo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yrmwicrs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gwmjyect.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vhvaulkq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hzciixto.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dqhfvvxk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ickpubtc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ejzdbknc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pcqwutdv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3aplglcgt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vhfsckfj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cdkuuiqn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3thzwtarz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ythuartf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3patlpndw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rrgzyexq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bboemgzi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wbqgjhig.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wyfycgfc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3apdseglw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwgocglk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nifemvzv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3tkflhpqk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gcmtvdks.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xpwczsqp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ynlwtsmf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vmfsqiyx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3asmergtf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scaesnxo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wyeevazq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bnfnuioo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jhudzzyr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ivrinldu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gvrcurpx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gjcnyjkp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cpodybwb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xszjwquj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bdnhqnbj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3stlktsye.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zkfmtjtd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3miasahxz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3dekfeyoi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jcguzxrx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3oxzqzrvo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3badbjmul.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mkmxatwq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ynwvelsa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pnxsysxb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tjuupura.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3keimfzso.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jrioniay.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ewkvjrzj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3erxcjwqs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wetswckg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3gngxlcnh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zxsnqdhr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rpatgsmi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3alkkkbst.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zqmwspgt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3pjypgqtn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3rimjdwta.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aqxuqipb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kbkntcyn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xyljgflf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3jjziymdf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3rzeawdzf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gcqprplt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3azlzwney.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rflopvio.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qphvnzyp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3heechkuo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rovfhxbv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hnubqyvo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3crkqnrqu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yxxnsren.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lscfmime.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bbwgklxu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xvppclah.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dywgpgny.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3gkpvjsdl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3eyxqwbqd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jcfvvowz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bhumrnwp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qeyrhrey.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rcetiphq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tisokfhx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ciwqewpz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zxkgisfx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gdqbtztt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3poeelaug.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3snmycfgg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3osgocley.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3smsjetqs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ohihggrv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3osdqjuom.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zbgyxbge.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3pgblqliv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3drbsehmn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dridvrjw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3htfrbtyo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hfypgndt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vgwmiwma.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qmilzilj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zlwajcvu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jvbnrvpe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pfldqgmy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3wmciyjio.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3dxcgxfat.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3iwykbgef.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dqtcamuo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tnygmwoj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wflbmgkf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nmykhinl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3sqqtseyg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3yvslkoqa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rgzcfaaz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ncbqruzx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pcwtwuwt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hwjkizkq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwvsnxju.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3aqgkmujg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kfsitbxo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ocfajcru.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gqqhmaij.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjapjemw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wxoytvtg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ymcbfllf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ucukaayj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wkaoosgc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nmmfxaub.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sactekuu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3brilnriv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bqqgcjol.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ktvggsya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvlfxdxd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pbvuoqfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xizmpfjn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cktmqwtt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3movydxip.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qkrmivhr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qlvjthow.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bdumpjif.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3khflhhoh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tuinwjuz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ymfrbeka.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qeydjeve.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qzmbednb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xjnjecli.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3bpacosmo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ewviykwk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cdxdyqul.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hxyyeaxn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pdhognkj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dzsnhacy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dojshcrl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ahmojhxp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3kbckhiwi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oegqlzlw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zupugubt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eobqpfex.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3znwlsgmc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cwpfpirg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3hrrtajqw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ntbfhceo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3onkrnplp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eukvlyyp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tcnyadgf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3exdlfavd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aldqpooe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vsizrdtj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xhgyonmt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uxfaavec.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oquyjzzi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3eddyjspc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jmsfsjzz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3azjuvsml.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wmmcjaym.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ogxjppca.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aaobdcrl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ihdcnrzv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kktotsnb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yrmkhtwv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kfuslykq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3usviaedd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pqcpyeed.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ynfzexlt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mnpqkcvw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xlslmdcw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nlzakclz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lmnvcron.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sjqkzqoz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mmaxcrha.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3udbfwzlb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eomcddiy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ukpgqueq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3toybqwso.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bxwqkknn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gxaxonkj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3svzbcdys.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bdyjzgdb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fwpxzmpl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zhyjcxta.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xnneazhx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tmymrmtd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mpfssyyq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rbashttn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3uetulhrt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qjzaigoj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nmbffvye.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xofofboa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zuwcmwge.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kwreuqbt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rqyanrys.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jdftohyc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3muevowup.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ountccei.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dcuyjkph.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yjxolbvr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3fterjmkh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gyhotcbk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kthboajl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jtbdwjiy.html


<!-- 参考信息 -->