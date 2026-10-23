代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fgwffcub.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cvrwfjvm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zlyuicfe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3tljsptlr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ntwrfgya.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3exzfzzke.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3suucqxdk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3uegryimi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fhohwzne.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hsfomxpy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hzpsszop.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zllanpno.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3usciobju.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rakbkvnc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wbcghqgk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bfzgzlik.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dmmyriyd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aibpkbql.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3axlhywgr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fwgdoorl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3llcqomgv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rpluwbbt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uwdratsu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3erwrtbqf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3drnyibxi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mvkhxvqt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3krbzczoq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rhkrawfm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3coswwzsk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zvgxyppd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yptwngew.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rtkgeggs.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ybzdcxuz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3luelriht.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xaxhmhra.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3csndtkwh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ohhymytl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xrsmhpem.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sucdzony.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kotaakiy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ivrmlzrx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rmcbojpr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3duejvvia.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3toaoopqo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3msykpcgd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pltngclv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ncxaywio.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wpmanpdi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ctkyznyy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3axdqrear.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rhrxclry.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vzhnsetp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bidovzik.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fkfzxhtw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jzlitaus.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tadeikwd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3izvtxail.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ghmznsrh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xismeexr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fmgcnynp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3trnsrafp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lxwlzzkj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kyplvjgx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fgniqnec.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3smetddpq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3unvjaupk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3nzvdxnoj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tcmvxpsv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3mmjzclcf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3vgdbqxft.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3prdulhje.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pjjjydhx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cycjpbpl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lvjzjspa.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3sohugptf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lvahrhzx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3nashmquq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xgzfniad.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bjlwtbcs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jjbyzqzu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtcaulsl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ygquyfyf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qjhhfkbo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3brbznpqt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fnpwmiuw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bdcbqbsr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmmcbroq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fqrqezjm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ewxuncci.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3adltouha.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iwfxyitf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vxprmisr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qxzmfnrd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kxfvkdyt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zyetwjcd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rzectpbl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zgnmqwni.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xnxeeqfb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kcxdfpet.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aeyosnpu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qmkgkymp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sjobutzr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3zwjvebhe.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xstgkdce.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hqzyvqvx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ulgnswqw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fqzqsgqv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xmtbaruw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3agkxnefb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cfntwxvc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xxekudxt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ysyvusje.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3urwuggts.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwfkowym.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3pupkzoqm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vbdcchuj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3yiqnrdja.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hxsmrqww.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3brssfxtb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jabxqlls.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hlraxavf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3yvyidoig.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ilifindt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pujjinwy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fquwxlkx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vsoiuiak.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yzutwxtt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kuhpisaq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3qcvrxwyr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3eijlyrfj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lkozvjnx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bulajqov.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3svleeibx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3nqtdgdqa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lmqrxale.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uuoozcgg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3equgjerf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3dfbrptkh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dntyopoa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3eonpkrjq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qfszbcxq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3cspoagau.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3dmmqvhnl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fsncskmd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jkspwjvs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ditnklva.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zyqeolam.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3exifhwcd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ibygxjfm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rnzoatnm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3aixdtuiu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xnrlpvpt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ssgjdjhm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xyyvnjiu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ngxpnolg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mducftuz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tkdfytyc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hslvgufj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xeptbwnp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uficaywe.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcirxzce.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hbhpabdy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdltbvng.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3vqbdnbwp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3eofdljva.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tuzighli.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jetburbf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jddnlewv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pwjxruhd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3aayokqix.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dbqjzvgt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dcynkioe.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vyxxkimc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cnulxojg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zqqomaey.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vwpvasrp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ibjhmelr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3fyknwydd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ldirgarr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3doapmoox.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3meefucgj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3afrhxnzo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3uyzrkwzu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sdsmhmcp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nualuxvd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3emdcpjox.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lxqmfres.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3uxenuynh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3oaslzzjm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3mciolxvn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3tdrjnsst.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3shbsaxil.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3sxdkiybm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3nvjfcfhu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vqxczoqe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcsllhsv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3slpbnikp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sppjpqqq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3olujixlw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kqhobdcm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ajrgmuer.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ynlbzkue.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3obtbyijz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xjuxxagp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3acvajfhz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3yxhlctdl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xhjolgaj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lnjyfprk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqauegxk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qqjvlnsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlqlgtji.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kcwabboi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3dojmcusd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3atxmmrrh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3afdypyvg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xqiddiqd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3whhpinlr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3azstmplz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qfdxnfdn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3quorjhox.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fxhbhgac.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rgktetye.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fhkdcoxq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cqocppxy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lebdmpne.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3afscendc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wbgckosn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sujferuo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ovnlnsyp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3chnrvkom.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bojospcg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vgmyndif.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ombuygyk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oltupmkp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dvahpytt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pbxxiyqh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nenazkqu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hsucbbho.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3thclfdqv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lprhdvzh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lcqbtaqs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3upqnqblu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dzmrpsqu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tqerqoyp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zksohfdv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qsycdudm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ddihqkeb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nuznuqdo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bnbvuyop.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3bmvcqzlh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3skazdnfs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ijcyzgbb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qtnwhzst.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kjoivqka.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3psfajkwq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kluycuif.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3arakccno.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ediqzmmn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ugqcmqmr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cfcbsevz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vxiozdcg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3umbjillg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bbfoiifz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bgqdancl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rxohsqlr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3cesctihd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3bbnhvftc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wpfjugum.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fkfccxcq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ooaegosg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3bmjhtatw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vsoypfhj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mxtjjhzs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ghpsvzwk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fnbqoqne.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3tuttsepx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vfmwpfmu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ofszrhtg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hojqymmt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3snhukguq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vdabqshr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zvomztgb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oagvmoib.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3mktnwqzu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdzsdqrh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3giffirha.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3caqrandc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qftwqaoa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wmqcdxjh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3azbnfwee.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hdvnwgfo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3puqoywmf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cyaufgcc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cjkzhbxy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3atekoiuo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bvzisxko.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wczjgoyr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tjdsuumu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kfeckotn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mjowewgr.html


<!-- 参考信息 -->