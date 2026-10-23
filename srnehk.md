代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pkbdgaue.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ovvrverm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dappdcki.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vopkwjuq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3kvwfzxox.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wigihduf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kohfrsjq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yksjrqpc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3igrkfpeu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3vczpsajt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3dpquzakn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kpoknekg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lgsoyhys.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hwyjlumv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3oiirkhjx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vzokipim.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yktxjnrd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jxbtbguc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3eucvwnya.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3cythhdre.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vbwqmash.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dwhmoikg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wzrsuxli.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3urueysay.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3exhvpbkh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vmpnjxcu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3uuavctan.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3wzfiegdx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ytvabmnr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3azbdbwqw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gezfuaqp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ivwftabs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vauiudhi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wdfpwjhp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nfyikcby.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bpbuwxfa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3guksfyqh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3eevjpveq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ynteigdb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xgtfgzcz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jqgghswd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3exichtbs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xpoqghfl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uinladpa.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hatzqsup.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3meepnihx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kwzkbwdq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3mcdbgpic.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rqfqgpvm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vnvazaou.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zyobkgkq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3thljhazn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3chpzzxuk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3givzlfdv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3habxpqak.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hqemytfj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ojxqagle.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kpxfenus.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tbtsfzbm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zrclfciz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ghulrgmj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3zhwaxumd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3nazxspqs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3dlkecdnc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jsyemccl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dhcvgyqu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gvwbkzqr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ejuivvfr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bqnqgqtj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ivaxizap.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3olemzhlw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3tiulfrpz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3iwkxgppj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fqrhochb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3aobepijy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vvzcdpdm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3loihqotn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zgdbtyrx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nhnmrmcm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zprrgace.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xlhavlur.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gcvvbtbq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tjjmiwyp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3wbyakmtk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3kugqlcjx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3bavswcis.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hkrnsscu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3zmkigsdb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cvvhtzic.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hrapmvna.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bkhbnbof.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dtvphwec.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3stecgqbm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3auwirmmf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ngoxnvws.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xipqnvju.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lybmzjgl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxzgtekj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mddnsduf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxnntkwx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3sowbrenp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ldbfsssf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wmczbgak.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mkxmzynb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mglgdnxp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kabkaboq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3oglahveq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gcsudyle.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hxvvsibd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3flrfkhfc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3koqirasc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hfxdagno.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mdayjago.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vmhdgqkk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebpzyqmn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3irfpkcst.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sbkmrdld.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3psmwpmsa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mchkfdrt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qhcxycex.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3togzrwcu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3btxczlgs.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijsikoha.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3udineqmn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cpmhygre.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bxmukmdt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3yyojsziu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lvykwjav.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sxmbicuu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3rdmvwveo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3siplepst.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qufmqzna.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3amkouanl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tjuscbsx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vwcuhmus.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3jicgnedk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3gozeqlaf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3uarrqnmv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3zpiewuzl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eteltabl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ltssozhv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3lyhyqgmw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ygjwmfqc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3khzwnper.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nypensle.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3tzxcwhbx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3caucjxzo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ofxpvdeg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3psyrwyvy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3gsgmjfkn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3caqgsqbx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jvypjvyg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kszbdbat.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vhxdqjkv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3syhglhws.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zmiwcziq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3slnmstgm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3odhktxaf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3sixoaeie.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dbxnvcup.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tjqmebga.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3szruduhp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3syzgmlxw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fvzzgqea.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3bwbvjvco.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xpvlitsd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fmuogemn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hsxvnxac.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zmffheoe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jilnuqms.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3wwomyckd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wwpjepfi.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3plvdfnzh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jllwnwpv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ipbnhpgy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3psnovlqn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3umwgoumg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qbarusdi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxjcuhr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3euxebnzc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cthdwwoj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cvemiphp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjggsgho.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3buqijzyy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lexmlutp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3khhkjwow.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ovhbythy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3lxyrzpyp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ybnxeifi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3oeivupcn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ghgzolwj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zgnmspec.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3eztltluq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fmshamsr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hlujyemm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mvfttdre.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3grvximga.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3iydjqfku.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gizhhlxl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3obtcvxhy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhgkuqnq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3uztgprcp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3iutrbeqr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dkchhcri.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aggxtlcn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mogysgxw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cfoxbpiz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3sqjozwqu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ceaaspxq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kivvqhxz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zibfbwpl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3atbfsuvt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xdgihbfl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3uwasuvae.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bzkrbsau.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lnhvxyml.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3xlmrizcu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3otrxvzkw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aqpyjgxc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3irmmboaa.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vignigfy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sppyhzus.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eilhwqox.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3axvfbiwf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3unayvdvx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qnyvemsl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yqdvriww.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wuhxpiam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3seokseqz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3abmjuqqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfeiprvk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ltmbnvwv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3nxrnpezf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zcrbrgsi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rokhqngl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bqwinxec.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3epfsferj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lknykweh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vvlquurp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yolrhckj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vhozghgx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qkmrigpv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pefaqvva.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wvxxkvta.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dijboylw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ijsfmjhh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3rqnkqxzd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gicokqnz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3llzkmupu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gyhoeqsn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ejdvwzwl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ijkxnwmt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yexygnby.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3krkimxzd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nwrzxbqb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3eshsmekq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3asrmdzsw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qtatfhwv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qtetepcn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xcbizati.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vnvssdke.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3znfkxbhm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rzwyaeix.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kkdynphk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3pkestkpf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vzjlpvoh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ehcumklb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hmmzyhgs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3uhepjkjm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xtwfysnz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3haointep.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3riajsnit.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zmikaxgu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hsdsjtxe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jcbqeqjn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ibgsfyuz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3cckkpnwl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cbktxvyq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ijthlpod.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ogdcyvhx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3srenppyp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3atnidzsx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rdmhljol.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xztdyspa.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zjvodkvj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fwsixwno.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3gflxytie.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pootjpwt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ychbfydl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hipmivws.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xlrnbrml.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3degrguvj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3nsfxrpjy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wqxuongh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3oucmsuil.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3rroctpmq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3aahkelzj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vkxgtqvm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bxhjxftd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qibfomuo.html


<!-- 参考信息 -->