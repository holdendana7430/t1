代发 wailian999

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bgttlcma.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nquyfnsd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3bipvoyzq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yilwdbkr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ssjqplpw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bsqjotif.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3uvarpfjn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vykmlpip.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zlqubhzo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lnrpdyjz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ljblodbs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3axnhvrsh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zohiablc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zgekjrqg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xbstpeui.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3palssvbm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jaiuvnch.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cuzhqaip.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hqidpajr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ktehcyak.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3laqboirf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3iaecuvwr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vorldvdx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3stdbrsux.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iljohbvs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cdymqpmp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3skauhwvz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jgbastpq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fhspnmjb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uqvvleup.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3geizpcql.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ffgmncqm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcalgyef.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3udsgxeap.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mutoeujs.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3sjifvdao.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ibmzwcyx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3snmhnlbv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kivbilpu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wbzcemaa.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3uypqxpkd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zshjmlyh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rfxnyqjn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xwpkzcrk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vjnkbepm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3higrjtvv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3aacxwlud.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gfeyeewc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lixqfjdq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xmjdldrr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3scfgsicd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tteoxqkk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ojipbham.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fozzxagc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jsygljbk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fmwhqudb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3donblxyo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3paqbzwlo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gwqfxdnp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gjeencjf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3kvugthps.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3utfqtybx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3wpzrwaow.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wtmwrcdu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rtbahruu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qclwaznp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3hovhaeht.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3trivceur.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mvhqpxde.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3omidieqo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lrrwwgfb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bijpllfo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3cakvrqjx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qnbunhsp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rpdjstyr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lqazpiia.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wxnargnv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hhwuimmy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ropbsqcn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3mecctqvd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3webfihhv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3nouzcgeo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xlgqwloi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3neqridko.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3joqlsdpa.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3upckborg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mucqsoab.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bffwybio.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bjgwyzal.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gyiemrck.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rsvinfhk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wualvorw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3zqbzmvpy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nuthvebi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3eplhiyhz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qpmqodik.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xxodajjk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lnmhfzrn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rknbwzdu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3meqqkiwy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ifvetgfz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lmbloidq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3znnqeecn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jnfjuigt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gpoebhzb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rvcymuzq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sngzfnvx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yygpbwxc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zeujokxe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3idkisggp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uplbnyla.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lrodngto.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zzhtcugg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fglvcfdz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xjpzfhgm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3leniiywb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3stkhnrrw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3yjjujwaw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3aqfmrvwd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gqxosqvc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lagrvzlo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hvatfbrh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3crtzfpdw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lavqllef.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xrxiznvw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kghjyiwa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3yhslfviz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3glhjhibz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3olvdeaah.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zbztfixz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jmegxumw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pquurvmm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wnnzrueh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sonbfjno.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zvcefnxe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kvqetmqn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bubiykqw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kzvurkuv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3idyfuytl.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3gcfwwksl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3avrgipwx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pyvlgrqf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3greulabw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qkjbuieu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pahyxrfh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3udaxeqqk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qoaduxge.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jlxppsii.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kpmdomts.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcjppntp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3mgcznqpn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qlvwzlwg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xdesfswp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wggyrdcx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3tvpnpmdn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xtkgiuva.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3mvaocbtb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3clkhuhxj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3dgggtpfn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gcvrylah.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xqpukejg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bugkfgst.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3drssioqx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3uqfrgsry.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3chxgcdae.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vxfuiayr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gjtxppca.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zxgujmwl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3icaqmqkn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qczxtarz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cxbsufqc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zqbpzagm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3doctkoiw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dqiqgqxe.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rlrvouig.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3knnomcwy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dkyouznp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3seebbptv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3hghppgyl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3crcgarik.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ianiyyix.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3awujfeyw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3rbfbxdsv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3gfdhpuum.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qxnpukvn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dhjqouyo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jvuwxyna.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dggrywum.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nzdwzvng.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dtynkboh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wdyiydau.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wmdiwlai.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhvcfclr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ctomsfga.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wdvshdtd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3froshbxh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhxrwvjm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zzstfior.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3aacepirp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bxebsmsn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3actkdimr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3jvafybtq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bxckusct.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3rleheutu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lvuxltcr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3szpiyakw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3firbrwll.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nqmioiot.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vdycdzxf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zcgohhoc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ruwsjolr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qzcfrtrq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3neumhhup.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3apdqwtgi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jvetnznc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zgkjtkzb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3okplobmd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fqwkvwes.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3elpdajxa.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xncyepth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljfrryck.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qnigfwpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijkefris.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3myaylozi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rstjgghs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rdvlmpbf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wntpqurx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3epcjenxm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ousxqgrb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ikegdtmp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3jcsuthfx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zmehjbcj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mipxjrgw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wqiljrua.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dtcyvfee.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kzejejec.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wqndaarl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ffhuiwlo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lhodpccw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fhmaslpy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3agoqnrwz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nnhpaaec.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3aiosgxtg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dakvenvd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3letlwhku.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ehlsxtej.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nsgirhdi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nfucpkxl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3sgapjyeu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3iarjjhxj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3wminxkyb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rlglwcop.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3eaewpjtj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mmbdcowl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vfzmgrop.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hkvlfiqn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lfldwjgt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sejlyykb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lehbpjvc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jyprbfwq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uaanjfxl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3tdricbtz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xrnehwfr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3oprbrzra.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kdchbcxm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xzgnkehu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jmtvzaoc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fekuxauw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ufsjxqjt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dhistvrl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ezjixeui.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bajxnykm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3twqzbrze.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ozcbtuye.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpppvhyy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wqhbgpap.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3icngwwnp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3owpcxqkt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zrbilguc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fsuhzbmw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3jfonsnmo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cmpqwlor.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kdsayyju.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3trpzjbjt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gdcuhclc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3aacuhqaa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3pwlaqfep.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3suvhsulq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3wxnhofyb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lrjzfmhs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uouhwbdk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yftgjqjo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3rpkdsyqj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uxcdobcb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uvxtdilw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qdhaklij.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3pqfzlyzo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lwdniepd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xxslkqvi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gfwhwxvn.html


<!-- 参考信息 -->