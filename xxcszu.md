代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3rycdmtjl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zrfxolte.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jrmyyiqg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bbnggexx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3iayeekjt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jdpvzkgg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tghyzdqs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tfrldema.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oklsptha.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jkoxiopu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wtadjayr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3prvwaiei.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gqzhvqgo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dadmlktt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3tbyuzkxi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3didkhqpu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pmqbdvdh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ccetpzfp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pkfdpxbv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3seixendx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xlpygcwn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3abzhwihd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rtcqxdul.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3afodtgvv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jtiehznu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ybdfkkdr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vqjejfjr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qycjqwaj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfyjdpu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3yegsanim.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ftwbcxbm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dyqeyrmx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gewwxysd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yysygahn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3knhcxeli.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xozymidp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zzbaxuba.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ggoqnowr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tkpwyqos.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qkpmkzvb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxtxbzui.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ledzhxat.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bndoycsf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ifmmvfwh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3pbfxvlkc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tifyvrgt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dtmlaauh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ugnubjzp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3jcybrrbj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3lwcqfoym.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mmlkimla.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wpvdamoo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xixzrjdk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oxizsdoz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3uqjpinxb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3oufznanw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uqwurgjn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wbqstgfq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rrqndrge.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3uqbtvdia.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3coynshjj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qntgjkyd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3bdqsdqpv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cxarrcwu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3panjndjj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wecytgtr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3uoynwgbg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3twkrucfd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mritwfwa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3fteufcbx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3oggsbwvs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3oexjghwa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xsrfkdqi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cmudlhhk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3nhblghlc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3uinrunzr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wzgoalcx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yxleiksg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3abbgielx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uwkijxwy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3aemhidhq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3eogqlikg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3xheyeing.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mjprycmr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3mgaysnae.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zparjbrv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3elcmfkfm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zcrvjzdp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3srqztjec.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bqpqqbhk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pffaymdk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3tyomutpm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qoavtalh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jwextoza.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lhzdwzfw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lwpiqrpc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lypeevqj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dqhzrxwf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zwvmgdcr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oaquwiwy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3getogtmi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vjdthxho.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vxicehbb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fnavsmpe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fzsonasm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pywrmnwe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rrhvyovj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3sctapaoq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3sywsfffs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3yqyevxxf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3suvyguay.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bhiheujr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nhxfavxp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wwkeshtg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hibvpffm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dgjhugjo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cthtbzbm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wkykhbmo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vhkriohu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qlcypnqf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dhibavru.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3srxormxo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ahopombc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fkmdijzd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vbysspsx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3izhmacgn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fkoymmnw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nbwsnqni.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3soywfsuh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ndfmovfx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hydgeqxd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vnwbvgrt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nuhjifkk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kfahdkmd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mngncyon.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gvyllagy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ennkjjvz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rigwtxcl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3eerubijp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ogbzbqie.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jljsfzcc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bnwjyqbz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qvlepqha.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yqdrossu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebsjfbld.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3spyogwps.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3gqozqvsy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3uwkfvuwa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zbpozmco.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3drgkdosh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3hnpxdfae.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3uejfbfgl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3lamwthrw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3couoldus.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3oybbvtxg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mizmpbhc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gcuyijak.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wmnyvhfv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hgkywakx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3igpowrvg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3romzsdmg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3oyxmysbr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ahifgivd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vtjbewgr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jqesnbap.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xpfxlcca.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3yyrvwwud.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3cuaaxhtu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jjgryqsp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zxrimmud.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zmckjsrv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3jdwwxewc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3gbkxviki.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fujbxaym.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3kdocvzjo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jioypgye.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mcfluxik.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qekaxruq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hsijikir.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3puqhkxqh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgqcdfzs.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pqjmmada.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bavolnsj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3lrkpnocv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3retavisc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3aaggnfpx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3rtimvcly.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3eyoyjvfp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3pjxtyxzp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rwmveqyh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3yanqichc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3itjxxgao.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mihaheaw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fxpoioom.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3txtkzoeb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jxfyogzg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gysgcdzf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3khalnumh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mrfhjuxf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3oliahwcl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3uelzftwb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wtyuspbt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fjawyrqd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3nuanhavi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ynjkylhf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ompzmcel.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3inznnmdd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3omqktlpz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lksfgbpd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mxwrpjey.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3usjcwwhq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jeflvjjb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fdillqdd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3slrroetu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zmxqxsxe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pnstcfbk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3bahjmokr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3shduxbyb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3najibkeg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3drnvvwft.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jqlpestt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fbkpblnq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mevfzcvg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3goskucnx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3favpwatf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ywplukya.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wxfmxltb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wpripvaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzbihcir.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3uvuhbdhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwmwwwdx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gqarnuzb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3iaxywnsu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kffjzjaf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3axurzoat.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fksvklxd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gtwamszp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ssfzmamg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3hmbejazg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3smeieclx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ifmiwscm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lccilfec.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ftkoenlp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vkrphjyu.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jyxamneh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xiyrgwrb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sggbhpsa.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wbsibzot.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qcrlqtnh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dxfttlfy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ldilbvpi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ourllttg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qrcbyvpz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cixupxcg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3buhvbuml.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3znbmxgwo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3foxcximr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rijlnoqb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ppkhywsp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rqxdehgl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kyvtpohg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mfltidii.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qdktewsc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jipwtscz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zqxiwtfn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nfbkrtzg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ljutfunx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mfkwlial.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jbirnnke.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nyenxwzj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ljfcpuwn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vsgfpfec.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tfkbjtfs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3afjbzclw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3watukecu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nqbjxvwx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kgncyeyj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fpanabja.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hmbdddmu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ziksulfp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zmjlunwi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ujrghpok.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3emhqvmdv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yjfqosny.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vojacoqa.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3auyisbpo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wqplfwmv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bpcwckkr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3acgmalyk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3dpjafsfz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dnbviwgd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tjxwpqjn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3nywbkjfw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ndeileoj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bqxrzcsq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3cddkbgxg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dvtoqugf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ltxayasa.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qhsyhbef.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bzcupenq.html


<!-- 参考信息 -->