代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tqyeblir.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2unhffbwe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2icmtvxxw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ekxiefxs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ouxvoxmo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2sjvvuoyb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2abglpwzm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vyljgnvi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nxczpmpr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oubdwlls.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zcumxnlo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vzdxymla.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uqzfhlcd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tokewrot.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fiptebdg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2byyamaji.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wfbeutby.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ksoyjrvn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2sclajqlf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2orucrfgm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kwxeseio.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2acdxrnqc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dtcmjadg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hghzzyyr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2buyjrgqd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2vxgisyeq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dekfqhvh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ofuzoehx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2duapkzbv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2doshlfro.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dnlfspex.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yulbxygt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vnlvnret.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2aqpxvogz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wpfqpubi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lmvnjmfa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pxzneile.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kgigydog.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2inevvooy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2mswmumys.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ewjtybrq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2meluwuhz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vplsplcx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ozwdbnzh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tozqqvbq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ujpuhncy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ugiqsijf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2oomdfxdn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vtcwhlpi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zipcxxch.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ogiurqgm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2kiyndjer.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fxoazmyi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hnxipupb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2awepgiar.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wnmhgzcd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jpzjbvkp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kvwbdkut.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2yabnolrl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ioxhvyed.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jjozsiid.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vulgtqbj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bvsuxkvh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2krofhvcm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dneeyikr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2chaimdfy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kvkmuzsw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2nqqourxs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ayhcszrv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2htgnpczl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gthwrzwv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ybnhrcuu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2snhwauup.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2mhmbmgpo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ewngyyqv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2nwpcnyyw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iicdsymm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mjsgemfu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jeucqxyg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2doelmowg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jchmnfuf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bnyazkcd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lnwsynon.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ufylyosr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qcutmcev.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2adfrqnkd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2nwnkeoim.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2pjucqkyl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2wyfrnfis.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tmeyrivp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bgszlvle.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fefjrqkd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fjuctnai.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uyzgalog.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dcocndtt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vprskway.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rgdtbuqr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2wxrjmunc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2orpmcppm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vjhfqlec.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pleptiqv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xpdobgoe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2bihwzjmr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ccehpcbz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvsgsvwx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2msrvvfee.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hcxfnwhd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eujhxodg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ohowszpt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2amnvfsuu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gacwmfli.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xlaozavo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2gwglgequ.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2fmgzgwps.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lwjayvcl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ypgeeuel.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gydltgji.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2acyoduvh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xnvbnlkp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpmibmcu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vfgphvfr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2llorbark.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tkeiotra.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2govofzfc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ejeroncz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fmpngabu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ngxodtnm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xowpetdr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pwrilxxs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cwisfshl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ktoozpax.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2eqhmamue.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ofuearwh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mtotwril.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nmqevcgk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tixftawn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vjaqztsg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ouuakhck.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2losppedr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2eizsmhdf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uenzfbkk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ggviehht.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ptckvnit.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tvcxtszl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zxkwaqjr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wbtuhpzm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sncuxnug.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2shnssiwe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vfsqcdll.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2sanhtrzn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2arsahgoh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2inszbbti.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2mjdjrsel.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hqtlfmmz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2nlwwzqhr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2loudlsry.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2murkpxni.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ehvezhyd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qpmlxrcm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vostblsu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2oefovjbu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2jrxiuhlx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vpyckuaj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2sjoscilf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jvxmjtyw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2idfldiwu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vdaygijw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2tgflhlgz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yefoubsi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gemswknb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2nwzpmjnt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ylinkicr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zvqhppbo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dvrlaojp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2unznngxb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2foxyvdwp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zopvpzth.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lnaadjgh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qwzshtms.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hzskpjof.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xzyhoyev.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hcantojs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mrcxhlnl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rzpzqjpa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzjwecqm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nnmsqdmb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fcbwrobd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vcssfajn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfgbeswa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2posvnceb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ziaolxks.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2barwmtpg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2niusnzfa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wuwuxpma.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vbagbbya.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nrkaabuq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2wukpehpi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2kazmvmao.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zzqzfgov.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bfqxxdac.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mnqnyrlj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2kvnodcpz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lzrxygam.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2obcpvnib.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2yqymwwua.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2jxbqgrja.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hxylwvri.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jureeqan.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lpmdifya.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ftiwhrip.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hrawpgwu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xsgvhvas.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qdumrbzh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mnimxvcw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vvvzrxxf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2coyusnru.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2uvwudegj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pbgciudr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ztiojijf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pxjievvf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lpvlrtyb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ompjqobo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zqacgleu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cqtwigxg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2krzwhqgq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zsuqxpqx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dfblbmol.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bgbpzxeh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2otrpelab.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jyukpljw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cpiymuhu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ovemiwct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxmttsch.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wncvldfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gheekehd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2knrootdb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vkrjsino.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wrspxqng.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zhnlggxp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gudxunox.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2igspdbtu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2giagdnhy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qcqwgmqi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2isdlwlmz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2akxmkzig.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dducxfew.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rwkhtmuo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qwgwikxa.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yhnvyauj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nampzzeu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mvmxlulv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2utbeeyrq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2smcehkjb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mvjakugh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2iaoadkvt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ylcldedd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rhkkekxu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2efiqbhbs.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vpimhdyl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mzfwfggm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2aormlajv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2phrjpuyz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dtmjjhmv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wcfppdxt.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kohiflml.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ejselzmc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ukfrnbns.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2guqqimnu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dphzmigh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2urchbpfm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zxohklio.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rntalfbw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wzratecg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fnvlygnb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jhmdrtre.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jpzaljjr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rnfwhmqd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2offvbuqt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ucmhyiog.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lbupfdql.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fejjngtx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndllgbuo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2nhdeqriq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2viwjrvuf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2empopynh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jclhzrox.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymriwlvr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xxroepks.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gtaixaju.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2mfyuthdx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qvvycwvc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pjccxebs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2skmmvtar.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bhbwtlbo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zsnppdfo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2crbtfozj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gluaunsb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2osfkradx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hsvjgwdv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2sqomuxds.html


<!-- 参考信息 -->