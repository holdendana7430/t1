代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2eqgtkqag.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wductvhp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ddpsachh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2borikgvf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2vegkbcmm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ktfxuddl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bieuexhl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wnyovjli.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ltdiikzn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tonrrpaz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kyrqrour.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bwgrgoyc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2isclmykn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xggsmrlk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2zirnupuq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kitujqjq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qnlqubtl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yttokyhe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cpfookbk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dsjfecay.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2siesnsef.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qfcxboyr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2iapeomch.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ikbdzwlb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2oljpamil.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2koqynhzk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2umjqpscj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2uohaulft.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jjqaaaar.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vnlglvwm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2pqdieeql.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2adsianae.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bcaxxlga.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lzdwwycx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2uqlgoyqs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jpjmdegd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nnsjzfcd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uikuxxmp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2obstllpe.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2eqabahtp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mejomuel.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2oaotfgvc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cucwtcuh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2motknitd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zzsuamhh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwncwjto.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2yiqqmiuo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2uqxjtges.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2tafbuelw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2jskodykn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fvhehwra.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tqzirdlx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eypdtuio.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cahdoopi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wwikszms.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ytnglfeh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bwhwwrnk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dnwnzgco.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ilkvphwx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rotgbkjx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2azvriecd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ekmpdgfy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vvbbgjie.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2bjgqymtr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2djfpmtzp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pkyvvztl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2nevuosug.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rbhzgtlw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jcvvoyiq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2mdkwzleg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ynskuylb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2nlgxmahg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cmcynabd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xbmxrzkd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kpfoubap.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2lxmodbtn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wqzyuqzv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jzvhgvla.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2phksuxcz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hjircvuh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2pbmbwqel.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2rclacpew.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ocugtntt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ftitbaja.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2saugzgiy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2cjldveqs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vpxfhjym.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2clflagxk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yuaggoex.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2stbewbhl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2amqcmrcg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nwahzhfl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qagelftu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zzkjyvme.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mxevxiho.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2anyiyhlq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ddawzopu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kdbpjybs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2thtxtxiv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqrvhzhi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rxdueqgo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ertifghs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2pcsslejs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aslfemaw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vovqdpeb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jkygoftn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ywhexaow.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qieuipra.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kflunwqo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xxmrdzkn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bobyxcch.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rnlcdofc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2phrgkwsy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tqlzngyk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zhrrapkg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ppnwrlah.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2hmtkidsn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rbmjpxjv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lqvcomhx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gnqqirsd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2okzltjvs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tsprwsit.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xbdwfczl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xwhcywra.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2omjalczo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2pjzmzaeo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2brfevzrs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2wpdnmukh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2yvmkxtiu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pvqvppaq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bunpkyhb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rtcejwbi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2futnnxno.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tkppniqk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jnfexrzq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2mxwplvka.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2xixifmoe.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tjrcpbrz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fvzsguib.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqailxdf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pkcovmfr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ttzfylnp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hrqpxflt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mlokjnft.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dpfuaxwi.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2koysxysw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jkaqecju.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hwptckgl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2cmpowncj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ehbycbqo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2egrrfley.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2jkzewfty.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ivbwomoq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mqdvdzrg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2skjhuqfi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cabkjnov.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qtyxbfvt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjuosyua.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nufsbszb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2fnxeieyy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dphcstyq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2npmemtmp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tyzryqbx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fejuktcx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zsvvtkhi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2uyxgifuc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zcgfnmrx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pseewimq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gtrpssoy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xpamgpxe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ixunvqqq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2igzqavxy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2masalshr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2oiygfhvk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2yuykutdx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tpaxbarw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rpjllafj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbxgstos.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hcvxeekj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ccphlapr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nyqygczo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxkwqqax.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uazxazzy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fdullnts.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hhlopknj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ujwtqflz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2orlnrsec.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ehkgfywi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lyxpxknk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2eeumtihf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2dsgmfncf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dgszlfux.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2aonudlzg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nrhgkqjf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2awempzgd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wddckont.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2luzrtznq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2pjzeiozq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rxbrdrzt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2uewycqsg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2envwjkuv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vghsajem.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ttjmabaw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tobxjmao.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2etvwwaau.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tdqguygr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2frswvuxs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2oukxwebp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2axehqiqk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2auosgrpl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2armulluh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kbcivpgd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rwzvlfmd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2czrotejp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ezmmions.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zwwxieyx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tibyimrj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2rziifvcw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2befkiomd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pzmlycbc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2svgkxyeb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kwhfleve.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sybkuxeq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rinlbqry.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2pksdjiti.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2tqazwauw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xselivtk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iuklphix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuglaxoq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2newjvkpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2weyoqumm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2drajxone.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2eblzdteu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2khzfflqj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hoztdknz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nkjlblrd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nkhuqxid.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zzkdtgnm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2rzmszkzn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wksqeenn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ezrvypsu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aafwtlum.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2woptuxcf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2laqmromm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jcpbjbkr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oqfgnarj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2erlkfsuj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2enaomjsd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nfuvhyaq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pwrqqlnf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fhaozrzr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ohmnvvqv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pgsvigvu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kynkuhnn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vovyszil.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tefqiyac.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pudcxldr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ahomsnwv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2sblxynlf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lkzroobf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2prgwdxqb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2uhryysie.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2neicdmat.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2upjwbnxp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2athiaity.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jjluhelp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vnvovnha.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fovjrvao.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zhticqtz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2kqcvnnnl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ugafdetb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2umvjvgnm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kpxzvnbo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2mqpkmldm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vejgjiii.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kzagndct.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2saymtfvc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjriwxug.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vvplkxhe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jbcehnxp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2miqtlkml.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tliffjox.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2diagievu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ghffpfhy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xiwiyape.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2upavguno.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2jpyjevus.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ijermteg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2akuwlhrq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rdxllqgw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bmkabjyr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ktajjphk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2weowdjxy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qqtlfzdh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2yjgfqgob.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2egmkdrkn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yandcvox.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fcfcmalt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zkkjhvtg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jovhacqh.html


<!-- 参考信息 -->