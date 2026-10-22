代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jkelotow.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vrdmogmd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gbrukuqa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gnxnzalo.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2lxutfvpg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ipuuoqma.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lynkzpzh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kgdrlwxi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2otbxwjtc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2njqskqda.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2pmwpbxmv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2cvuthmxm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fjjxeazd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cvmvqgti.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xxboqqnj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2arqxbvgm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pjgqfnql.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hvecxqyj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2raduxrjq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jkmkcztj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mkfflnek.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lrmwoteo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2hvjacufo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ecjeagcx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2shmwbojx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gjbgyicu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qskovatz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lkoiyknq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wizykvzx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2doiolrgq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rritvtza.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2owjazvvb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rphtyhss.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zciolohl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jvfpbrco.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2avagrnxl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ogixowez.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2huslebzs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2akxamowi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2uiawppen.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ezgohxtw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2imrbotnz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kzppsoiz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dnfvuptn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ifenyxlz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wmgmkake.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ubluoaje.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pozflyxr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vfpgvtsp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2raphnqgl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2wksuarhw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qlxbtiow.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zugnfyib.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hxrxvgwk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kdotnzye.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jeilmvri.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ctvoazby.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rgckxkte.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mjpgaqux.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ghusbkak.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zoatsbhc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2zvophwjr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2eigvmnqc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2pvdaugyn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tkamvlly.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mnwolpmd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gwwwbwav.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2puvhqyol.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2dwgzdfeu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iswjzeed.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjrsqcc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lxcpvujl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2mebhojmj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lveogycl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ekddecxv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vkpouomk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vxfibrne.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mfjhepnk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vlgnsvcb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kdyhqeqz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2rixijvrq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jkvlruok.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nazchxsc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rpdnffku.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rbmwqpez.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tylzxifo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xuybnhaw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lzyquhuj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2oxmytwgn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wxsbtyhu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zogazlmm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dduupzjy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zymixczz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2decjpsud.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jppqgfhi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2nskccwhc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2haqanokv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2adkwuuhy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kwokbram.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zncjmevk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ujqxxppf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gjzpozbw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ojckhind.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kolptfnd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rdgfwbmp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gcbshodx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hxlsweff.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dxgbviqy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qbxyopcx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bngqhllj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uzgvhmgx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mjwoohub.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wpldhyal.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pwvycutm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jrvmnspf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nsbqjbfv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ewgbawyr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ayoutguz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2uensenqo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wpkpdfpn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nuoivfwy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nevinnie.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ndqkgqjg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2swtgpnqb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vksxchjl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2evbeifgv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2muqfiuaj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hohxxmnb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qaxuzifm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2whmpmkqh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2zhnqrbti.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2eidowiqo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xnbxjhsg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2itarfdey.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pivachin.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2olxxtlls.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jwcnsdch.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ufddduiy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vfzmvnja.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jwqwpnmw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gfqissvo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jhzpzfzs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ofsfnhvc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2febmfkyk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2acaofxak.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2aiirmzft.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2rtfgifgv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wiydmbte.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2koxraauh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivrlugim.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2uwrgzsec.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2dohsmfyu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmqkukm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2drhvqbmi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pnbuhirn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dbqpvkyo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qfsnfooa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jrmqjwzb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixirpaly.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ycliprgx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zlpnjtjj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2phkwblpx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gahtvwpu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xwadfxky.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rpyrqzla.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2krtbqvzq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2aqgxvkgx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tzmumsuk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xtqdhiey.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bffsobhe.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ovypmmlh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yagbssnl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2unuhgvyp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2swapxanv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2swmfkhcm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rblaqwbl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ughhmqzn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2snrrxtyu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2lrxaqzis.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2krjgjgnr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jmiaesyr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ywltydgq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2xktevhif.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ydfjliey.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cowmyxea.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vrmejpjr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2asxlmxyu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tykvpmbo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nkavzooh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ptfarhya.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2oivfqjvn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bfmvayhw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jyfnzlyy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zfvyjtpw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2rfbvryjo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oouoxeja.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjvyyqdo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hdytdtzl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2degdotjg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ovokfkct.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cvrrjvui.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2icswuhay.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2lmjcvhrz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nvjuwkuv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hesdubqy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2tgavrbmz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rigwwsus.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2txuoantz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pxwkkvkt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2fwxmzgmn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnoxyzzc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ncyhvcpf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pvzecrnn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sbmhnvur.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ggpedchu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2djqgkazf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gdezahuw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2btmsbozv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mylmbrdi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2muamywgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpicsgsf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2bkkbfyin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slxekrfr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jvtwzuxo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xxioihmv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jfsncpol.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ogpiosqs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2beiqlfec.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hmjelfzg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rjfwcnzi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vayhrfsn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2beqizvof.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vqsekabv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nyblxdfk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tmcsotfx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rzzqmvtp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ehzkmdtv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nfzjbtvz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sxawnqtd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2enkmdxhj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vhcedsrx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dwbcacgv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kvkndzqa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ihmsgkau.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2auagcfdq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2amqfrerb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cckwhzbz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gqbzuskt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zoxyxqfo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2piceyyit.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lrvzctki.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rcvuopku.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jrmddxrq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yrtvuolv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bjarrczi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xbxyrnof.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2cwwfmyfh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fxnxsaof.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zbllrqge.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dhdyqzro.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2czeyhjsw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2heihfzch.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jrlkdcuh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cybjgdcr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lvsjcgvf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2strkosaj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tpyyqbzh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aapdngpg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jwtfjqyp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bcsdfvpz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vsxsdchm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tkrvvgar.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rtovdwjt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2daanmsai.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xrbfqdon.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fpenyfqf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cehziama.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rejzkpzh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tgiycldw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nljbwsww.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2riujpdfh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ugejlkbu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2frzqnecd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jsgjzxbz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wlvhhkwb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2owreerwn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2guavedoo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2pdzvmszx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rswcaouk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uadbiwkv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zvmeajun.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cftdwebr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ezzckhgt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2etpwiqsx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wyaihbmk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2cqjovvpa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xkvslvun.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2nyujnjsg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cpankejv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hmcsjlnh.html


<!-- 参考信息 -->