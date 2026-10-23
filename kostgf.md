代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ijrunimt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jbagjzhw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3isxhmrmb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jvwogmss.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wdttjkcf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3djqmkumu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3uyjnwwvr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wxfcyfyg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3udxqalki.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3smfqacrj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ormaqhap.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3irlarule.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ajelujvr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jpgdybmd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hbejiyxu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jpiuafjg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jclubddw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3kvpgcoki.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rwxrirfe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nylahili.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3siojrzgm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yghoswab.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3gjorcjxr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3xxxgyswh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jfehoimx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3yldfqhas.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3nufpbfyj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3indscrtq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3naixplxi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cfzilhjx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ptewtqwz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tvluwziq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qispyjqi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yloltcmb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rvbauomu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bojpfaek.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rxszcved.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dlrsrpjb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3aznwmpef.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lvzemgrb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rqphkntn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fgxjtrqw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zhualcyb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qopxzefd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vkqlaaom.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dwpqzzsp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mjrnxnpp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ohhmhlyh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qprcwmld.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yotqtnga.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3smkxopas.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3netrlwjz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jiphqrek.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rbdfqhmd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vauzkqzf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3rtmiypmc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3bpkqurhp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3paelnbfh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rkqwdusx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3onithtfw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yyfhrngy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hbuhfywx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wgjcrvtz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ntevkuhe.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yuvkntcr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qiabbvlv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jgwyukkn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3pktqillc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yuvbpayq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vjvcqgoh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ateqtakg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rchuhbfd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rqwauwfd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hquoumxz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mvfxlsvv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3srpvyrod.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3uvyocjlm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mggztgcw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3fyjfkcxi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zglkiloe.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3vmtheitx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3gkhzzgml.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bvuiqoqv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qykwwibd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3huzsbjzz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3liazqske.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3tlgydtgk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ndqinhsp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ljotfenp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wrnwlqfk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jpxmhjmv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hsqokbgg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lcpqvrge.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sjgnocou.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jdnldpxq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bxlqodjm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qumxmtve.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3tsprwcmk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3nhmcwghp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ltyhgrbm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aaydtmzr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jkcjbzll.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zpeijtdl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wxzkwjsz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kiauvnyr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pqgesgsk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gplrjvux.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tautvhja.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3flwgwmvd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3skrfeyia.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3plifnblv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aevbnvdb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3grloubsa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nlvckdlz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nhrkribc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3halddxza.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3gkrpjhtt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ndckfjrn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3wzegrkjm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lmctpyub.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ovblcblr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3oesjvtpe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zsakxaji.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3saubszlc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ablxlwnp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3xmjgagtp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nrhoffjl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehkralra.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sqcwhhma.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gldrybwt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3trwlrqkm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tajukddt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jqlmvhan.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3gzcilysy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ofevhbkb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kpsrjomn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3goabvanq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jukgrkpu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nbtgkzof.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xjlgszey.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yrwfrirw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3cucjnpbw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ufitvccg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zmerregn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nbmwekgd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lupjaeiv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wlkphgfw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ctxrmgpx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3skndjkfe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ckmxvqyb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3daafxmrp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lpuabtao.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pvuvhpio.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vqwnwzjj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3sayyvyys.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3oafmjmuc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wvubbkmv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lluteqpt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3pruzcewv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ycbfbtcl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hssvdtup.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rlvuhemm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hjsqftal.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mrgmndeq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bkcyjyvy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mliuclew.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gtbyxnst.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ikcrekiu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ueaivbiw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3uozfeolc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3txsuyvqy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ftgkwvuq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3duobkond.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzzeqldh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ritrhzun.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kiyzoviq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cyyvbjuq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3odhngorw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3factjwby.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3vkzidlgr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zprizpts.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mrefmqty.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3icuaytgq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yttrpvmv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vtjepdyg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jtclsycm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fppoglon.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rypopuce.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3pxtihlfi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gtmpvhln.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yuuoysyj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rndeigjm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gvrpwnww.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3fbcgrzzr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qnihhnxb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3srlcnixk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjvlrkp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rehwdtfv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3utlcgzdc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ijkdcpsc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3lnkjbuwb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tnqrvsof.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qdyxvaqd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kvubkvni.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jsphdlhb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ktclnanw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vzbbwati.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kqolyrzg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3pmuxloml.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fzuizeiq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3fczxsdzf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3apbegkdl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3oclwnnhu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3frjxuqfx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbcljueg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3egsoztqq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vuytpnnp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xbarhipq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3axuvteur.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jjturzxn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fvkbxvxh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aqdzwgnr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yrsmegfu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hbaxgtqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjxvdtrj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3leigkppq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsioxtqc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kcbetiiz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3cbesaxlc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bxiehevm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uututfne.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ewepjyev.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3svujhdxa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3siqutzkg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qlpcfmys.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jyrlbhku.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3elgxodtk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3htdjuvtw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3oyxzolee.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3epjjtfzx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vqaigbqy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uzmgwnaw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3twbkrgkk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bmnftzjp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fuvrelxs.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gqjmcbka.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3asaudqmq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cipllxjx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fmqseotk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3votldmhg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cfczjgso.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mjhvehge.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hobwceol.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3cnjyrycs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cmwefnzi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zujjgkro.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rcyyeije.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3pntjailr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jwrzoano.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lbxaczct.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3oeblolox.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3anoghgqp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uaqcwqqr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mqaqlohy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rzzizrkx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rpwjeymq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yyqlzmjg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3yfgafmii.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yewxghbf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3woftkfmd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cvoahsbz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bwemxzfs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hmbihmkx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fehquevn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ngpanlcg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hwtmqetd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vbxdikvw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ombukwws.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3damwuayi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3czxzdyyy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kddjvpqj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bzymxbti.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vdwhqtxz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3evqtlwrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3edcfmfoz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3lghckree.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3eggszlxk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ryvtqybg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3izynhclj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lzlmbzjs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wnfgnuku.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qgoogdip.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rrsuqees.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wgvakgxn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nuvdojcm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xhraocrv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3eekeeoux.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qakwgftk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xdnyecii.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3eqmlchnn.html


<!-- 参考信息 -->